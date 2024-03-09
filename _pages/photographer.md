---
title: "안녕하세요. luna song 입니다."
main: "false"
layout: splash
permalink: /splash-page/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/image-filename.jpg
  # actions:
  #   - label: "Download"
  #     url: "https://github.com/mmistakes/minimal-mistakes/"
  # caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
excerpt: 
intro: 
  - excerpt: '앞으로의 포부를 여기에 적어보자 `type="center"`'
feature_row:
  - image_path: assets/images/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
    title: "Placeholder 1"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "placeholder image 2"
    title: "Placeholder 2"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/unsplash-gallery-image-3-th.jpg
    title: "Placeholder 3"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
feature_row2:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Left Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row3:
  - image_path: /assets/images/image-filename.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Right Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row4:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}

{% include feature_row id="feature_row2" type="left" %}

{% include feature_row id="feature_row3" type="right" %}

{% include feature_row id="feature_row4" type="center" %}



feature_row3:
- image_path: /assets/images/about/super-snapper-zIwAchjDirM-unsplash.jpg
  alt: "Career"
  title: "Career"
  excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`'
  url: "#test-link"
  btn_label: "Read More"
  btn_class: "btn--inverse"
  feature_row4:
- image_path: /assets/images/about/mockup-free-SD9WHTV4uxY-unsplash.jpg
  alt: "Portfolio"
  title: "Portfolio"
  excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
  url: "#test-link"
  btn_label: "Read More"
  btn_class: "btn--primary"
