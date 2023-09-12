# [Quantum Group Website](https://quantumghent.github.io)

This website is powered by Jekyll and some Bootstrap, Bootwatch.

Forked from the [Allan Lab](http://www.allanlab.org) site. Code released under the MIT License.

## Seminars

### Math rendering in .YML files 

Be aware! In order to have math in the calendar and seminars box in the homepage, you need to use \\( ... \\) instead of the usual $$...$$ in the .md files. In general: double all backslashes. This is because in javascript the single backslash is used for commands so this will totally fuck up the page. 
The same holds for the news box on the homepage.

## Team

To adjust your profile on the *Team* page, go to the **_data** directory, and choose the corresponding .yml file (phds, zap, ...). In there you can write your **name**, some **info** and an **image** (make sure to add the correct extension). The images are taken from the **_images\teampic** directory. Preferred aspect ratio is 1:1. Don't make the pictures (file size) too big. Larger pictures have currently been scaled down to 1024 x 1024 pixels. Smaller images have not been upscaled.

## News



## Homepage slideshow

In **_data**\carousel.yml you can choose an **image**, a **caption**, a  **subcaption**, and finally a **link** that the central button will send you to (a paper, a news article, a research topic etc.) Images are taken from the **_images\carouselpic** directory. They are automatically resized to height 300px, so make sure your image has the right dimensions. TODO: 1. 1 adjust font, fontcolor etc.

## Thesis topics

Printable versions of single thesis topic pages are available at https://quantumghent.github.io/thesistopics/YYYY/YYYY, where XXXX is the year the topic was proposed, and YYYY is the **file name** (not topic title!). For example: [quantumghent.github.io/thesistopics/2023/JBridgeman1](https://quantumghent.github.io/thesistopics/2023/JBridgeman1)

