# 1D Computing Basics

Solution for 1D challenge.

## The Challenge

Create a simple static website that displays a table with three (3) columns. Each cell will show a picture. You find the pictures in the folder named images within the website folder.
You do not need to know any html for this project. A ready made index.html is in the website folder. There you find all elements and the first pictures included already.

There are more than 150 images, way too many to include them one by one in the website. You will have to write a Shell script that writes a new index.html for you. On the way you will have to deal with pictures that don't show up correctly on the website. 

## Tasks
* Create a README.md in your repository where you document your project, answer challenge questions, and let visitors know how to use your code.
* Create a working branch (other than Master) that you use to push your ongoing work to. Commit and push often to not lose work.
* When you are done open a Pull Request from your working branch to your Master branch, do not yet merge it.
* Serve the sample website (index.html) using darkhttp and port 12345 and display it in your browser.
* Exchange one of the images in the sample index.html and see if you can display that in the browser. Did you need to restart the server to do that? Why or why not? 
* How can you look up the process ID of your server? Document the command line used and the output.
* Write a Shell script that creates a new index.html which includes all images, using HERE-docs where applicable. Make sure that all images can be displayed correctly. HINT: recode may help.
* Show your understanding of Shell control structures like loops and conditions.
* Once you are ready to submit your work post a link to your repo as a submission here.
* When you have received feedback, fix things that are broken and then merge your working branch to Master.

## Description
These are the following steps to complete the challenge:

* Created a repository (1d-computing-basics), then made a README.md in current repository. 

## Usage

To generate an index.html file, run the following command:

```sh
./index-generator
```
The output of this script is a html file which should be served by web service (darkhttpd):

```sh
darkhttpd . --port 12345
```
to see result, open a browser and type `localhost:12345` , then press enter.
