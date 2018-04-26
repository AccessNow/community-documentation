---
title: Converting Markdown to InDesign and vice-versa
keywords: documentation, markdown, InDesign, documentation workflows, HTMl, PDF, Git
last_updated: April 26, 2018
tags: [documentation, articles]
summary: "The client needs to start a git-based documentation workflow and currently their documentation is based on InDesign."
sidebar: mydoc_sidebar
permalink: import-export-indesign-markdown.html
folder: mydoc
---


# Converting Markdown to InDesign and vice-versa
## How to export and import InDesign documents into Markdown

### Problem

The client wants to switch to a git-based documentation workflow using Markdown, 
but at the moment their documentation is based on InDesign and they will need to export Markdown to InDesign also in the future.


* * *


### Solution

The goal should be to use Markdown on git as the source of the documentation by default. This will make version control possible and facilitate collaboration.

1. To achieve this, the first step should be to export all the InDesign
files to Markdown, going through HTML.

    - [This page explains how to export InDesign to HTML](https://helpx.adobe.com/indesign/using/export-content-html-cs5-5.html)
    - Once the HTML files have been generated, converting them to markdown requires
Pandoc. Help the client install Pandoc following [this guide](http://pandoc.org/installing.html)
        - There is also a [web version of Pandoc](http://pandoc.org/try/)
        - Some markdown editors like Atom export HTML into markdown
        - Assuming the HTML file that needs to be converted is named `file.html` and the Markdown file the client needs to generate should be called `file.md`, the command to convert HTML to markdown is this: ```pandoc -o file.md file.html```

2. Once all the HTML files have been converted to markdown, the client can start
updating their files directly in the git repository.

3. Markdown files can then be imported into InDesign going through HTML whenever the client feels they can consolidate one version into a PDF or print.

    - To export Markdown into HTML Pandoc can be used again, but also editors like Atom or ReText export markdown into HTML.

    - This time the command in pandoc will be: ```pandoc -o file.html file.md``` ( assuming the Markdown file that needs to be converted is named `file.md` and the HTML file the client needs to generate should be called `file.html`).

    - [A howto for importing HTML to InDesign](http://networkcultures.org/digitalpublishing/2014/05/15/import-html-into-indesign-via-xml/)
        - Instead of the Python script included in this article to delete new lines in the HTML file (which doesn't seem to work), we can send the client [this script in
bash](https://github.com/AccessNow/helpline_documentation_resources/blob/master/scripts/sed-clean-HTML.sh). The script can be launched on a Linux machine (it should also work in a Mac terminal).
        - Instructions for the client:
            1. Download the attached file to the folder where you have saved your HTML files. You can open the file with a text editor to check that all is ok. You can also find the script here: https://github.com/AccessNow/helpline_documentation_resources/blob/master/scripts/sed-clean-HTML.sh
            2. allow the script to be executed, by running this command: chmod 777 sed-clean-HTML.sh
            3. run this command on all your files: ./sed-clean-HTML.sh filename.html


* * *


### Comments



