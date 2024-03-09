---
title: "Github 블로그 제작"

layout: archive
permalink: /blog/
author_profile: true
sidebar:
  nav: "docs"

---
코딩에 코도 모르는 멍린이의 좌충우돌 깃허브 블로그 만들기.

홍익인간의 정신으로 
고군분투 끝에 만들어진 결과물을 저와 같은 초보자에게 쉽게 설명하기 위해 페이지를 만들었습니다!!

{: .notice--info}
아참! 저의 블로그 Jekyll 테마는 minimal-mistakes 입니다.😘


## ✅ 블로그 제작

{% assign posts = site.categories.blog %}
{% for post in posts %} {% include archive-single2.html type=page.entries_layout %} {% endfor %}