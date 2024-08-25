---
title: "데이터구조와 알고리즘 중 데이터 구조만 "

layout: archive
permalink: /data/
author_profile: true
sidebar:
  nav: "docs"

---
![image](/assets/images/dataStructure/dataStructure.png)

* 추상 데이터 타입 (Abstract Data Type) : 자료 구조를 설명하는 데이터의 타입
* 자료 구조 (Data Structure) : 추상 데이터 타입을 실제로 구현한 결과




## ✅ 자료 구조

{% assign posts = site.categories.data %}
{% for post in posts %} {% include archive-single2.html type=page.entries_layout %} {% endfor %}