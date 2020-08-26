---
permalink: /features/
title: "Features"
classes: wide2
#header:
#  overlay_image: /assets/images/unsplash-image-1.jpg
#  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
#  actions:
#    - label: "Link to somewhere"
#      url: "https://github.com"
feature_row:
  - image_path: /assets/images/xyz.jpeg
    alt: "xyz"
    title: "Big Feature 1"
    excerpt: 'The latest version of libGDX, 1.9.11, was released on 22 July 2020. Among various fixes and improvements it contains support for Linux ARM builds, which allows libGDX apps to be deployed on Rasperry Pis.'
    url: "/gdx_1_9_11/"
    btn_label: "See the full changelog"
    btn_class: "btn--primary"
feature_row2:
  - image_path: /assets/images/xyz.png
    alt: "xyz"
    title: "Big feature 2"
    excerpt: 'LibGDX has a very active community on various platforms. If you are looking for a place to start, our Discord server is most definitely the right place.'
    url: "/community/"
    btn_label: "Find out more"
    btn_class: "btn--primary"
feature_row3:
  - title: "Cross Platform"
    excerpt: "Publish your games on Windows, Mac, Linux, Android, iOS, BlackBerry and HTML5, all with the same code base."
  - title: "Open Source"
    excerpt: "libGDX is licensed under Apache 2.0 and maintained by the community. Contribute today!"
  - title: "Feature Packed"
    excerpt: "Comes with batteries included. Write 2D or 3D games, let libGDX worry about low-level details."
feature_row4:
  - title: "Super Fast"
    excerpt: "Heavy emphasis on avoiding garbage collection for Dalvik/JavaScript by careful API design and the use of custom collections."
  - title: "Documentation"
    excerpt: "Learn libGDX inside out on the Wiki, study the Javadocs, or read a third-party tutorial. Learn from example code and demos."
  - title: "Community Support"
    excerpt: "Get great support from a big and growing community of game and application developers."
---

[ToDo, see https://libgdx.badlogicgames.com/features.html]

{% include feature_row type="left" %}

{% include feature_row id="feature_row2" type="right" %}

{% include feature_row id="feature_row3" %}

{% include feature_row id="feature_row4" %}
