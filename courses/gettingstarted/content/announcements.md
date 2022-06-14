---
layout: page
title: "Creating Announcements"
course: "gettingstarted"
unit: 3
---
Git Courseware features the ability to add announcements to the course homepage. These announcements will be displayed on the page in reverse chronological order and can be subscribed to with an RSS reader automatically when viewed. 

Announcements function just like pages, with a few exceptions.

## File Naming
Announcements must be placed in a folder called ```_posts``` that must be located as a subfoldder of each course folder. Announcements are named ```YYYY-MM-DD-title.md```, where ```YYYY``` is the current year, ``MM`` is the current month, and ``DD`` is the current day. The title may be anything.

## Front Matter
The Front Matter for an announcement appears as follows:
```
---
layout: post
title:  "Post Title"
excerpt: "Post Excerpt"
---
```

The **Post Excerpt** is the text that will be displayed on the homepage below the title. If no excerpt is specified, the first paragraph of the Markdown will be used.