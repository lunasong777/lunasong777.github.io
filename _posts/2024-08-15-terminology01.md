---
title : "SSR 서버사이드 렌더링, CSR 클라이언트 사이드렌더링, SPA 싱글페이지어플리케이션"
excerpt : 서버사이드 렌더링? SSR, CSR etc.. 히스토리를 통해 알아보자
sidebar:
  nav: "docs"
categories:
  - terminology


toc: true
toc_sticky: true

date : 2024-08-15
last date : last_modified_at
---

# 역사를 통해 해당 용어를 알아보자.

## 1990년대 정적인 사이트 Static Site
- 이미 만들어져 있는 html 파일이 서버에 배포되어 있음 (ex) home, about, menu)
- 링크 하나를 클릭하더라도 **_전체페이지_**가 업데이트 되어야하는 하는 단점이 있음
- 화면이 깜빡거리는 현상
- 버튼을 누르는 이벤트 같은 건 없이 단지 책을 읽듯이 볼 수 있었음

## 1996년 iframe 태그 도입
- iframe이란 html에서 또 다른 html 파일을 불러와 삽입 할 수 있었던 기능
- 서버에서 문서를 받아와서 부분적으로 문서를 업데이트 할 수 있음
- 단점 : 보안 취약, 불편한 ui&ux, html의 방대한 코드량을 넣기 때문에 브라우저 메모리 부하가 심함!

## 1998 XMLHttpRequest ⭐️
- fatch API 원조
- 페이지 전체가 아닌 필요한 데이터만 JSON 형태로 받아 올 수 있게 되었음 👏🏻👏🏻
- 그 데이터를 <b>자바스크립트</b>를 활용하여 동적으로 html을 만들어서 부분적으로 페이지 업데이트 가능

## SPA (Single Page Application) 싱글 페이지 어플리케이션  
 - fatch 서비스가 2005년 공식적으로 AJAX 서비스로 명명됨
 - Gmail, 구글 맵 등 웹 어플리케이션 만듬
 - 한페이지 내에서 필요한 부분만 업데이트하여 마치 앱을 사용하듯 사용이 가능하게 된거임!!!!


## CSR (Client Side Rendering) 클라이언트 사이드 렌더링 
 - PC 성능도 좋아지고, 자바스크립트도 표준화가 잘되면서
 - 커뮤니티를 중점으로 리액트, 뷰, 앵귤러 등 라이브러리, 프레임워크로 점차 발전하면서 CSR 시대로 넘어 옴
 - 클라이언트 측에서 다 하는 형식
 - 서버에서 우선 인덱스라는 HTML 파일을 클라이언트에게 보내줌
 - 그리고 또 서버에서 자바스크립트, 리액트 or 앵귤러 or 소스코드 등을 또 받아야 함
 - 그리고 또 필요한 데이터는 JSON 형태로 자료를 받아서 클라이언트 측에서 동적으로 HTML 을 만듬
 - 단점 : 처음에 접속하면 빈 화면만 보임, 자료가 무거워짐에 따라 몇 초 걸릴 수 있음
 - SEO(Search Engine Optimization) 최적화 불가능
 - 장점: TTV, TTI, 인터랙션이 가능


## SSR (Server Side Rendering) 서버 사이드 렌더링
 - 웹사이트에 접속하면 서버에서 필요한 데이터를 모두 가져와서 서버에서 HTML을 만들고 -> 그 HTML을 클라이언츠 측에 보내줌
 - 장점: 첫 번쨰 페이지 로딩이 빨라 짐
 - 단점 : 블랭크 이슈 -> SSG 때처럼 어째뜬 서버에서 html을 다 만들어서 가져오는 거라 화면이 깜빡거리는 느낌을 받는다.
 - 서버의 과부하가 올 수가 있음
 - 자바스크립트를 받지 못한 상태가 된다면 사용자가 클릭 이벤트 발생시 동작을 하지 않을 수 있다.
 - TTV는 빠를 수 있어도 TTI는 늦음



## SSG (Static Site Generation) 정적 사이트 생성자
- SSR 서버사이드렌더링 처럼 서버로부터 완성된 HTML을 받아오지만, HTML 파일을 생성 시점이 '빌드타임'
- 핵장점 : 생성이 완료된 HTML 문서를 재활용하므로 응답 속도가 매우 빠르다.
- 베스트 라이브러리 React: CSR 특화되어있지만, Gatsby라는 라이브러리와 함께 사용하면 SSG!
- Next.js : 강력한 SCR 라이브러리였으나 SSG 지원도 함
 <hr>

### TTV (Time To View)
사용자가 콘텐츠를 클릭하거나 로드한 후, 콘텐츠를 볼 수 있게 되는 시간까지의 간격을 측정. <br>
즉, 사용자가 페이지를 열고 실제로 콘텐츠가 보이기까지 걸리는 시간을 의미


### TTI (TIme To Interact)
사용자가 페이지가 로드된 후, 웹사이트와 상호작용을 할 수 있게 되는 시간까지를 측정. <br>
이는 페이지가 완전히 로드되어 사용자가 클릭하거나 입력할 수 있는 상태가 되는 시간 
