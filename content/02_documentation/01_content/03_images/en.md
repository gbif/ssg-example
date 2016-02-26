---
title: Images
description: How to create responsive images
category: Documentation
subCategory: Content
---

# Responsive images

```styledYaml
images:
- title: Măguri-Răcătău, Romania. Photo by Dorel Gnatiuc
  url: /images/mountain.jpg
  link: //unsplash.com/photos/rlXgUH7Sh_I
```
/images/mountain.jpg
//unsplash.com/photos/rlXgUH7Sh_I

You can insert normal images in markdown, but if you need larger images that scales with the device you can insert them using Yaml. This allows us to wrap then in a div and use bottom padding to control the height. The image will now keep aspect ratio as well as fit the screen. And the page won't jump if the image is loaded on a slow connection.

```highlight
images:
- title: Măguri-Răcătău, Romania. Photo by Dorel Gnatiuc
  url: /images/mountain.jpg
  link: //unsplash.com/photos/rlXgUH7Sh_I
```