---
layout: page
title: "Creating Course Pages"
course: "gettingstarted"
unit: 3
---

Now that we have our courses created, we can start to work on course content. Course pages are created in the folder for the course, and may be created in subfolders as well. All course pages are in Markdown format.

Create a new course page by right-clicking on your course folder (or subfolder) and selecting "New File". You can name the file anything you want, except for spaces or special characters. Lowercase is recommended (GitHub Pages is case sensitive). Files should use the suffix ```.md``` for Markdown.

At the top of the file, add the front matter for a course page:

```
---
layout: page
title: "Course Page Title"
course: "coursefoldername"
unit: 3
---
```

```layout``` will always be ```page```. ```title``` is the title of the page, as you want it displayed at teh top of the page. ```course``` should match the course folder name. ```unit``` is the unit number where this page will be linked from, based on your ```courses.yml``` entry. 

Below the front matter, you can add your page content in Markdown format (or HTML, if you'd prefer). For the HTML nerds, Git Courseware uses Bootstrap 5, so all Bootstrap semantic elements are supported. 

## Figures
Git Courseware has a figures module built in to ensure that figures are easy to integrate. To add a figure/image to your page, add the following code:

```
{% raw %}{% include figure.html image="imageurl" alt="Alt Text" caption="Figure Caption" %}{% endraw %}
```

In this case, ```imageurl``` should be replaced with the URL to the image (while you should add the image extension here, we use the same relative path structure as ```courses.yml``` - relative to the course root). **Alt Text** is the text for assistive screen reader devices. This should describe the contents of the image such that someone who cannot see it would know the contents. **Figure Caption** would display below the image.

For example, the following figure:
{% include figure.html image="content/github-education.png" alt="Github Octocat logo holding an apple and a pointing stick." caption="GitHub Education's Logo" %}

is generated with the following code:
```
{% raw %}{% include figure.html image="content/github-education.png" alt="Github Octocat logo holding an apple and a pointing stick." caption="GitHub Education's Logo" %}{% endraw %}
```

### YouTube Videos
Git Courseware also features a helper for embedding YouTube videos. To embed a YouTube video, get the video ID from the YouTube URL (the last part of the URL after the equal sign)

{% include figure.html image="content/youtube-id.png" alt="A YouTube URL with the video ID highlighted." caption="YouTube Video ID" %}

and use the following code:
```
{% raw %}{% include youtube.html id="videoid" ratio="16x9" title="Video Title" %}{% endraw %}
```

**videoid** should be replaced with your video ID. ```ratio``` has three accepted values: ```16x9```, ```21x9```, and ```4x3``` for widescreen videos, ultra-widescreen (movie) videos, and old-style square videos respectively. ```16x9```` is the default if an aspect ratio is not specified. **Video Title** should be the name of the video as you would want it to display on your page.

For example to display the video in the image above, you would use the following code. Note that aspect ratio is not included because I wish to use the default setting of 16x9:
```
{% raw %}{% include youtube.html id="w3jLJU7DT5E" title="What is GitHub" %}{% endraw %}
```

This would yield:
{% include youtube.html id="w3jLJU7DT5E" title="What is GitHub" %}

