---
title: Front matter
description: How to the add the required meta data to a markdown file
image: /images/lake3.jpg
imageTitle: Description of image and possibly creator.
imageLink: http://myLink.to/Where/Credit-Goes
category: Documentation
subCategory: Content
---

# Front matter

_The article content is written in markdown. But we need some meta data to know what to do with the file. This is added as so called `front matter` in the beginning of the file._

## Format
This data has to be at the beginning of all files. Notice that it starts and ends with --- . It should include as a minimum include a title.

* title: This is required and is displayed in menus
* description: is a good idea as it is used when the users search
* type: what kind of file is this? Can have multiple values.
  * [none]: this is the default. The file is a normal article.
  * menu only: This is a navigation category, not page. So "Examples" and "Documentation" would on this site be examples of files that only cary information about a site structure.
  * link: not a page but a link (likely to an external page). Requires 'link' property to be specified
* link: http://www.myexamplepage.org - if type link, then link to this location
* drawer: should the article display a table of contents. Can have multiple values. default is `false`
  * true : display the drawer
* style: [none] | myclassname . If present it will be added as classname(s) to the article. seperate classes by space.
* draft: true | false. If true then it will not be visible.
* image: show an image over the markdown content
* imageTitle: Does the image have a title 
* imageLink: credit or link to original source 
* category: will display category name above document. Will also be shown in search results. This should be the name of the parent menu/folder
* subcategory: same as category, just a level lower.


### Example of an article
```
---
title: Front matter
description: How to add meta data to a markdown file
style: article mySpecialPageClass
drawer: true
---
```

Example of an article that is still in draft state
```
---
title: My test title
description: I'm still working on this file
draft: true
---
```


Example of a menu only file
```
---
title: Documentation
type: menu only
---
```

Example of an external link
```
---
title: Wikipedia
type: link
link: https://en.wikipedia.org/wiki/Main_Page
---
```

This page looks something like this
```
---
title: Front matter
description: How to add meta data to a markdown file
image: /images/lake3.jpg
imageTitle: Description of image and possibly creator.
imageLink: http://myLink.to/Where/Credit-Goes
category: Documentation
subCategory: Creating content
---
```
