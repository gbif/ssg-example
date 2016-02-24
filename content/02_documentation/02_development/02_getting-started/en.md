---
title: Getting started
description: What to remember when creating a new site and what options there is for customizing.
category: Documentation
subCategory: Developer
image: /images/building1.jpg
imageTitle: Cityscape. Photo by Padurariu Alexandru.
imageLink: https://unsplash.com/photos/ZKBQmgMyf8s
---

# Getting started
After the site is installed you want to customize and [add content](/en/documentation/creating-content/introduction/)

There are several things that can be customized

* [Style](../styling)
* [Overwrite templates](../overwrite-templates)
* [Custom templates](../custom-templates)
* [Language versions](../multi-lingual)

Below is a list of things that you should consider.

### Things that you should do when setting up a new site

* Update the `package.json file to have the right description, authors etc for the new project.
* Create favicons and place then in '/src/favicons'
* Add custom icons if needed (for example logo) to '/src/icons'. To replace the existing logo you need to overwrite the stylus variable that points to the logo. Icons should be .svg
* Edit the language file to reflect the languages you will support. `./content/languages.yml`
* Add content in `./content/`. TODO more about folder structure and article format/options
* Add translations of the basic site wide phrases. This is done in `./translations.yml`
* When you like you site and it works with the libraries you might have included extra. Lock your dependencies using `npm shrinkwrap`
* Set up build hooks. For faster deployment when editors push it might be a good idea to only reinstall dependencies if the package.json file has changed. The `buildcontent.js` script is intended to help with that.

Secondary you need might want to

* Overwrite stylus variables from core project. See https://github.com/gbif/ssg/blob/master/src/stylus/_variables.styl for available variables. [Read more](../styling/).
* Add custom css in `./src/stylus/`. [Read more](../custom-elements/).
* Add images you need to `/src/images`.
* Add custom js to `./src/js`. [Read more](../custom-js/).
* Create custom templates for usage inside you makdown content files. Custom templates should be located at `./src/templates`. [Read more](../custom-elements/).
* Overwrite default templates if needed at `./src/templates`. To see what they should be named see the [core templates folder](https://github.com/gbif/ssg/tree/master/src/templates)