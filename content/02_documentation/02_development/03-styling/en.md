---
title: Styling
description: How to style your site to make it look glitzy
category: Documentation
subCategory: Developer
---

# Styling

The css is preprocessed using [Stylus](http://stylus-lang.com/).

The default index file is located at `./src/stylus/index.styl` should look something like this:

```
@import "iconfont/gb_iconfont" // import iconfont that is build from the provided svgs in ./src/icons and the ones inherited from the ssg project
@import "variables_overwrite" // your chance to overwrite variables.
@import "../../bower_components/gbif-ssg/bower_build/stylus" // The core stylus files
@import "main" // Your own styling

```

## Add classes in markdown
In the individual markdown files you have an option to add a class to that article using the `style` attribute.
 

```
---
title: Front matter
description: How to add meta data to a markdown file
style: article mySpecialPageClass
---
```

