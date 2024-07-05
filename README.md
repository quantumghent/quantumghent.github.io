# [Quantum Group Website](https://quantumghent.github.io)

This website is powered by Jekyll and some Bootstrap, Bootwatch.

Forked from the [Allan Lab](http://www.allanlab.org) site. Code released under the MIT License.

## Seminars

Seminars are added by adding a file to the **_seminars** directory. The file should be named with the following format: **YYYY-MM-DD-Title.md**. The file should contain the following front matter:

```
---
date: "YYYY-MM-DDTHH:MM:SS"
speaker: SPEAKER NAME
affiliation: SPEAKER AFFILIATION
title: "TALK TITLE"
type: {seminar, jointseminar, colloquium}
abstract: {true, false}
---
```
If the abstract is set to true, it should be written below the front matter, and will appear on the seminar page.
If the abstract is set to false, the abstract will not be displayed on the seminar page.

### Math rendering in .YML files 

Be aware! In order to have math in the calendar and seminars box in the homepage, you need to use \\( ... \\) instead of the usual $$...$$ in the .md files. In general: double all backslashes. This is because in javascript the single backslash is used for commands so this will totally fuck up the page. 
The same holds for the news box on the homepage.

## Team

To adjust your profile on the *Team* page, go to the **_data** directory, and choose the corresponding .yml file (phds, zap, ...). In there you can write your **name**, some **info** and an **image** (make sure to add the correct extension). The images are taken from the **_images\teampic** directory. Preferred aspect ratio is 1:1. Don't make the pictures (file size) too big. Larger pictures have currently been scaled down to 1024 x 1024 pixels. Smaller images have not been upscaled.

## News



## Homepage slideshow

In **_data/carousel.yml** you can choose an **image**, a **caption**, a  **subcaption**, and finally a **link** that the central button will send you to (a paper, a news article, a research topic etc.) Images are taken from the **_images\carouselpic** directory. They are automatically resized to height 300px, so make sure your image has the right dimensions. TODO: 1. 1 adjust font, fontcolor etc.

## Thesis topics

Printable versions of single thesis topic pages are available at https://quantumghent.github.io/thesistopics/YYYY/XXXX, where YYYY is the year the topic was proposed, and XXXX is the **file name** (not topic title!). For example: [quantumghent.github.io/thesistopics/2023/JBridgeman1](https://quantumghent.github.io/thesistopics/2023/JBridgeman1)

* To use mathematics in thesis topics, double \$ signs are required


## Publications making use of QuantumGroup@UGent software packages

Publications, preprints, theses and packages that use QuantumGent packages can be added to the software page by adding them to **_data/usingPkg.bib**. Be sure to add a **year** field to all non-Package references. 

URLs should not need to be added to publications, as they are automatically added from the DOI. They should be added for thesis type references. **DOI** and **eprint** fields should be added to publications. For example:
    **doi     = {10.1007/s00220-023-04781-y},
    eprint  = {2211.01947}**.

Github links can be added using a **github** field, for example: **github = {lkdvos/CategoryData.jl}**.

A set of example references are included at the bottom of **_data/usingPkg.bib**, which can be copied. Be sure to create a unique citation key for each reference added.

## Events

Events can be added to the `events' tab of the website by adding them to '_data/events_and_conferences.yml'. Format instructions are given at the top of the file.

Past events do not need to be removed, they will automatically be hidden from the website at the end of the month in which they occur.