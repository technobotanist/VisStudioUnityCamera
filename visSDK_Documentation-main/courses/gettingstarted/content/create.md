---
layout: page
title: "Creating a Course"
course: "gettingstarted"
unit: 3
---
We're now ready to create our courses/texts. GitCourseware supports an unlimited number of courses. 

## Create the Course Folder
The first step to creating a course is to create the folder where all of the course files will live. In the ```courses``` folder, add a new folder (if you're using VSCode, right click on the ```courses``` folder and select **New Folder**). The folder should be all lowercase and may not contain spaces or special characters.

## Create the Home Page
In your newly-created course folder, add a new file. The filename may be anything, but should end in ```.md```, as a Markdown file. Conventionally, this file is called ```index.md```, but that is a best practice and not a requirement. In this file, add the following content:

```
---
layout: unitlist
title: Replace this with your course title
course: foldername
---

Homepage content
```

The content between the ```---``` is called the **Front Matter**. Front matter tells GitHub Pages how to render a page. The ```layout``` item should always be set to ```unitlist``` for a course/textbook home page. This means that a list of units/chapters will display at the bottom of this page. ```title``` will be displayed at the top of the page. ```course``` should be set to match your course folder name exactly. 

Below that, you may add any homepage content you would like. You may use Markdown or any HTML you would like. 

## Add courses.yml Entry
Once the directory is created, edit the file called _courses.yml_ in the __data_ folder. Again, as YAML files are picky about spaces, follow the template exactly. 

Here is the current entry for the template:

```
gettingstarted:
  title: "Getting Started Guide"
  shorttitle: "Getting Started"
  homepage: "index"
  announcements_title: "News and Updates"
  units_title: "Section"
  alert:
	type: danger
	message: "Git Courseware is now avaialble for use!"
  units: #Do not change.
	1: #Unit number
	  title: "About Git Courseware"
	  home: "introduction/about" 
	  pages:
		- title: "Introduction"
		  url: "introduction/about"
		- title: "Introduction to Markdown" #Page Title
		  url: "introduction/markdown"
		- title: "Software Tools" #Page Title
		  url: "introduction/tools"
```

The very first item, that currently reads ```gettingstarted``` should match the name of your course folder exactly. ```title``` and ```shorttitle``` are the title for the title bar and the navigation bar, respectively. ```homepage``` should be the name of the homepage you just created. Page URLs should not include ```.md``` or any other file extension.

```announcements_title``` and ```units_title``` are optional parameters that will rename the section called **Announcements** and **Unit** respectively. ```announcements_title``` should always be plural whereas ```units_title``` should always be singular. If removed, the default labels will be used. 

```alert``` can be used to display a message on the top of the page for each page in the course. ```type``` has four potential options: ```danger```, ```success```, ```info```, ```warning```, which will display the alert in red, green, blue, and orange respectively. ```message``` is the message that will be displayed in the alert box. ```alert```is optional, and the alert will not be displayed if it is removed.

### Units
A unit is a chapter/section in your text. Units fall in the ```units``` section of course ```courses.yml``` file and are numbered sequentially, starting with 1. Each unit has several attributes. ```title``` is the unit name as you want it to display on the course home page. ```home``` is the first page that users will be brought to when they click on a unit, which is typically also the first page in the unit. The ```pages``` section should list each page in your course unit. The ```title``` attribute is used in the nav bar and the ```url``` is the relative URL for the page (see below).

#### ```courses.yml``` URLs
For all URLs in your ```courses.yml``` file, all URLs are relative to your course folder and **no not** contain file extensions. For example, if you have a file in your course folder named ```index.md```, your relative URL is ```index```. If you have a subfolder called ```unit1```, and then a file called ```content.md```, your relative URL is ```unit1/content```. It is not necessary to include a full path or a file extension - GitCourseware does this for you. 
