---
title: "Splash Page"
excerpt: Bacon ipsum dolor sit amet salami ham hock ham, hamburger corned beef short
  ribs kielbasa biltong t-bone drumstick tri-tip tail sirloin pork chop.
date: '2016-03-23T11:48:41-04:00'
feature_row2:
- alt: placeholder image 2
  btn_class: btn--primary
  btn_label: Read More
  excerpt: This is some sample content that goes here with **Markdown** formatting.
    Left aligned with `type="left"`
  image_path: /assets/images/unsplash-gallery-image-2-th.jpg
  title: Placeholder Image Left Aligned
  url: '#test-link'
feature_row3:
- alt: placeholder image 2
  btn_class: btn--primary
  btn_label: Read More
  excerpt: This is some sample content that goes here with **Markdown** formatting.
    Right aligned with `type="right"`
  image_path: /assets/images/unsplash-gallery-image-2-th.jpg
  title: Placeholder Image Right Aligned
  url: '#test-link'
feature_row4:
- alt: placeholder image 2
  btn_class: btn--primary
  btn_label: Read More
  excerpt: This is some sample content that goes here with **Markdown** formatting.
    Centered with `type="center"`
  image_path: /assets/images/unsplash-gallery-image-2-th.jpg
  title: Placeholder Image Center Aligned
  url: '#test-link'
header:
  actions:
  - label: Download
    url: https://github.com/mmistakes/minimal-mistakes/
  caption: 'Photo credit: [**Unsplash**](https://unsplash.com)'
  overlay_color: '#000'
  overlay_filter: '0.5'
  overlay_image: /assets/images/unsplash-image-1.jpg
intro:
- excerpt: Nullam suscipit et nam, tellus velit pellentesque at malesuada, enim eaque.
    Quis nulla, netus tempor in diam gravida tincidunt, *proin faucibus* voluptate
    felis id sollicitudin. Centered with `type="center"`
layout: splash
permalink: /splash-page/
feature_row:
- alt: placeholder image 1
  excerpt: This is some sample content that goes here with **Markdown** formatting.
  image_path: assets/images/unsplash-gallery-image-1-th.jpg
  title: Placeholder 1
- alt: placeholder image 2
  btn_class: btn--primary
  btn_label: Read More
  excerpt: This is some sample content that goes here with **Markdown** formatting.
  image_caption: Image courtesy of [Unsplash](https://unsplash.com/)
  image_path: /assets/images/unsplash-gallery-image-2-th.jpg
  title: Placeholder 2
  url: '#test-link'
- excerpt: This is some sample content that goes here with **Markdown** formatting.
  image_path: /assets/images/unsplash-gallery-image-3-th.jpg
  title: Placeholder 3
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}

{% include feature_row id="feature_row2" type="left" %}

{% include feature_row id="feature_row3" type="right" %}

{% include feature_row id="feature_row4" type="center" %}