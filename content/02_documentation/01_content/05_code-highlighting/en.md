---
title: Code highlighting
description: How to get code highlighting
category: Documentation
subCategory: Content
---

# Code highlighting

Code highlighting with [Highlight.js](https://highlightjs.org/). To enable add `highlight` as language to your code block.

```highlight
var gulp = require('gulp'),
    del = require('del'),
    config = require('../../config').clean;

gulp.task('clean-all', function (cb) {
    del(config.all).then(function () {
        cb();
    });
});
```
There is no default style though, as that could vary per site. So either add it to the build or load per cdn by overwriting the empty template `cdnStyles.html`. For example

``` 
<!--./src/templates/cdnStyles.html-->
<link rel="stylesheet" type="text/css" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.2.0/styles/tomorrow.min.css">
```

See [style examples](https://highlightjs.org/static/demo/) and [cdn locations](https://cdnjs.com/libraries/highlight.js/)

