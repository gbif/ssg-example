---
title: Getting started
description: Get started writing content
category: Documentation
subCategory: Content
image: /images/taipei.jpeg
imageTitle: Taipei City, Taiwan. Photo by Eric Huang. 
imageLink: https://unsplash.com/photos/r75qppvP-FE
---

# Getting started

Unlike cites that use a content management system like Drupal, Joomla, Sitecore etc to handle the content, this site is generated from text files. 

Each text file becomes a page on the site. And the site structure is decided by the folder structure. This is many ways make it robust and simple to understand - for both developers and content editors.

## Example
Lets assume that you want landing page and an about page. To do this you would need to create two text files and a folder.

```
./content/en.md # This is the name and location of the landing page file in english
./content/01_about/en.md # The about page 
```

## Files and folders

The site structure is generated on basis on the folder structure, folder names, file names and file content. You should follow some conventions.

### file name
All files should be named by their language. So english pages should be named `en.md`, danish pages `da.md` etc. The file is just a normal text file with another extension. 

### file location
The files should be placed in a folder with the name of the page. you should prefix the name with a number. The number decides the ordering in the menu.

Example 
```
./content/en.md
./content/01_about/en.md
./content/02_contact/en.md
./content/05_download/en.md
```

Avoid spaces in folder names. Use `-` instead. The name of the folder (start number exluded) will be the name of the url address.

### Deep pages

```
./content/en.md
./content/01_about/en.md
./content/01_about/01_features/en.md
./content/01_about/future-plans/en.md

./content/02_contact/en.md
./content/05_download/en.md
```

### File content
All files must start with a piece of [front matter](../front-matter) followed by the text. The text will be interpreted as [markdown](../what-is-markdown).
