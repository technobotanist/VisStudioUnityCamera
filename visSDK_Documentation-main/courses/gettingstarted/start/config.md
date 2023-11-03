---
layout: page
title: "Step 3: Configure Your Site"
course: "gettingstarted"
unit: 2
---
Once you are able to edit your repository, it's time to change some of the basic settings that control the look and feel of your site. These settings are located in the ```_config.yml``` file that is at the root of your site. Open the file, and change the settings indicated. Once you save and push your files to GitHub, they will impact the look at feel of your site.

The first two options ```remote_theme``` and ```plugins``` are static and should not be changed. They tell GitHub Pages to render your site using GitCourseware. 

In the section titled **Site Information**, the ```title``` attribute will control what displays in your titlebar. ```style``` defines the theme for the site. The only two options currently are _ncstate_ and _generic_. Additional universities will be added over time, via a pull request on [Git Courseware](https://github.com/mjsamberg/git-courseware), or by emailing Mark Samberg directly with a link to the branding guide for the school or university. 

```nav_showcourses```, if set to _1_ will display each course in the header navigation bar with a dropdown menu for each unit. If set to _0_, the header navigation bar will contain a dropdown menu called **Courses** with a link to the home page for each course.

Under the **Header Pages** and **Footer Pages** sections you can add links to display in the header or footer navigation bar.
They are listed under the ```header_pages``` and ```footer_pages``` elements in the following format:

```
- title: "Wolfware"
url: "https://wolfware.ncsu.edu"
absolute: true
```

As YAML is particular about spacing, be sure to copy the spacing from the existing entries when adding new entries. The ```absolute``` attribute should be _true_ if the link is to an external site and _false_ if the link is to a page within this site. To construct a link within this site, start with a ```/``` and then point through directories to the file and change the _.md_ extension to _.html_ (i.e. this page would be ```/courses/gettingstarted/start/config.html```).

Save the file and commit/push to GitHub. You're now ready to build a course.
