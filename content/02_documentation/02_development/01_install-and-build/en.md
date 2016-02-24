---
title: Install and build
description: How to install a fresh site and build it with Gulp
category: Documentation
subCategory: Developer
image: /images/building2.jpg
imageTitle: Financial District, Toronto, Canada. Photo Matthew Wiebe.
imageLink: https://unsplash.com/photos/VviFtDJakYk
---

# Install and build

The easiest way to get started is to either copy this site or use the more basic example included in the [SSG](https://github.com/gbif/ssg) project.

## Install
To install dependencies run
```
npm install
```

## Build
Builds are done with [Gulp](http://gulpjs.com/).

### Development build
To run a development build. Teh default build is a development build.

```
gulp
```

### Production
This will minify assets and wont start a server
```
gulp --production
```

