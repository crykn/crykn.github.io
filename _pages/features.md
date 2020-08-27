---
permalink: /features/
title: "Features"
classes: wide2
header:
  overlay_color: "#000"
  overlay_filter: "0.3"
  overlay_image: /assets/images/index.jpeg
  caption: "Photo credit: [**Florian Olivo**](https://unsplash.com/photos/Ek9Znm8lQ1U)"

intro:
  - excerpt: 'libGDX is an open-source, cross-platform game development framework built in Java. Unlike many popular editor-based platforms, libGDX is entirely code-centric, offering developers fine-grain control over every aspect of their game. It is the perfect place for exploring ground-up implementations, built on top of lightning-fast OpenGL, and distributable to Desktop, HTML, Android, and iOS.'
feature_row:
  - image_path: /assets/images/features/crossplatform.jpeg
    title: "Cross-Platform"
    excerpt: 'LibGDX offers a single API to target: **Windows, Linux, Mac OS X, Android, iOS and Web**. Developers can use various backends to access the capabilities of the host platform, **without having to write platform-specific code**. Rendering is handled on all platforms through Open GL ES 2.0/3.0.'
feature_row2:
  - image_path: /assets/images/features/reliable.png
    title: "Well proven"
    excerpt: 'The libGDX project was started over 10 years ago. Over the years, libGDX and its community matured: nowadays, libGDX is a **well proven and reliable framework** with a sound base and documenation. Furthermore, there are plenty of games built on top of libGDX, many of which are open source.'
    url: "/showcase/"
    btn_label: "See some projects"
    btn_class: "btn--primary"
feature_row3:
  - image_path: /assets/images/features/ecosystem.png
    title: "Extensive third party ecosystem"
    excerpt: 'LibGDX offers a very extensive third party ecosystem. There are numerous [tools](/dev/tools/) and frameworks that take a lot of work off the hands of developers. [Awesome-libgdx](https://github.com/rafaskb/awesome-libgdx) is a curated list of libGDX-centered **frameworks** and a good starting point for anyone new in the libGDX world.'
    url: "https://github.com/rafaskb/awesome-libgdx"
    btn_label: "Check out awesome-libgdx"
    btn_class: "btn--primary"
---

{% include feature_row type="left" %}

{% include feature_row id="feature_row2" type="right" %}

{% include feature_row id="feature_row3" type="left" %}


  - title: "Open Source"
    excerpt: "libGDX is licensed under Apache 2.0 and maintained by the community. Contribute today!"
  - title: "Feature Packed"
    excerpt: "Comes with batteries included. Write 2D or 3D games, let libGDX worry about low-level details."
  - title: "Another Great Feature"
    excerpt: "But is it?"

  - title: "Super Fast"
    excerpt: "Heavy emphasis on avoiding garbage collection for Dalvik/JavaScript by careful API design and the use of custom collections."
  - title: "Documentation"
    excerpt: "Learn libGDX inside out on the Wiki, study the Javadocs, or read a third-party tutorial. Learn from example code and demos."
  - title: "A Great Community"
    excerpt: "Get support from a big and growing community of game and application developers."
