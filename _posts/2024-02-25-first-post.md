---
title : " Github / Jekyll 블로그 제작 (window 11) "
excerpt : 깃허브를 사용하기 위한 사전 준비 단계
categories:
  - blog
tags:
  - blog

toc: true
toc_sticky: true

date : 2024-02-25
last date : last_modified_at
---

## ✅ 사전준비

1. **Git hub** 계정등록을 한다.
2. **Git bash**를 다운받는다. (깃허브 서버와 로컬 컴퓨터의 연결을 위해 반드시 필요함)
    
    > **Git bash 정의** : window와 mac의 운영체제가 달라 명령어가 다른점을 극복하기 위해 만든 명령 프롬프트
    - CLI (command - Line Interface) : 글자를 입력하여 컴퓨터에 명령을 내리는 방식
      (= 명령 프롬프트, CDM가 비슷한 역활)
    - GUI (Graphical - User Interface) : 마우스를 통해 메뉴, 버튼, 아이콘 등을 클릭해 명령을 
       내리는 방식)
    > 
    

## ✅  Git 설치 방법

1. 컴퓨터 운영체제 확인 
2. Github 사이트에서 새로운 **Repository**를 생성한다.
3. Repository 이름을 설정해준다.

<aside>
💡 반드시 [username.github.io](http://username.github.io/) 이런식으로 만들어주세요.
공식문서에 따르면,
저장소의 저 username부분이 사용자 이름과 정확히 일치하지 않으면 작동하지 않을 수 있으니까 꼭!!! 올바르게 설정하라고 합니다 :D
그리고 Add a README file도 체크해주세요! 안해도 상관없습니다만,
나중에 remote를 해줘야하니깐..그냥 하는게 편해요!

</aside>

1. Clone 하기
- Code를 클릭 후 HTTPS 복사한다.
- 복제하고 싶은 경로로 이동 후에 마우스 오른쪽을 클릭 후 Open Git Bash here 클릭
- Git Bash 명령창이 열리면 아래에 명령글을 입력
- 다음 명령글 입력하면 index.html 파일이 폴더에 만들어짐

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/b30867a8-6abb-45a7-af6c-52033e167ab9/a102a19f-8895-4762-a107-4a913a315648/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/b30867a8-6abb-45a7-af6c-52033e167ab9/2df44005-690a-4c39-8a68-f4f6e4a866ca/Untitled.png)

```jsx
git clone https://github.com/lunasong777/lunasong777.github.io.git
```

>> 로컬폴더에 README.md가 생겼으면 연결 완료!

이제 해당 로컬 폴더에서 index.html을 만들어보자. 만든 후, 

1. 
2. 

Git Hub에서 index.html이 형셩되면 연결 된 것 맞음
- 명령창에서 아래에 글을 복사하여 붙여넣기 하자.

```jsx
cd [lunasong777.github.io](http://lunasong777.github.io/)
echo "Hello World" > index.html
---------------------------------------
```

1. Push : 로컬에 있는 파일을 git에 넣는 방법 : git bash를 통해서

```jsx
git add --all
git commit -m "Initial commit"
git push -u origin main
```

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/b30867a8-6abb-45a7-af6c-52033e167ab9/36e86d4f-3aec-4707-8ad3-a40d96f4d6ad/Untitled.png)

## ✅  **Jekyll 블로그를 위한 환경 설정**

Jekyll를 설치하기 위해서는 루비가 설치되어 있어야 한다.

1. 로컬에 루비를 설치해주세요. 
루비 다운로드 : https://rubyinstaller.org/downloads/
2. 다운로드 완료 후, 명령프롬프트를 열고 해당 `ruby -v`를 입력하면 루비 버전에 대해 나온다. 나오지 않으면 설치되지 않았다는 뜻
3. 명령프롬프트에서 해당 `g`e 를 입력하여 실행해주세요.

## ✅  PUSH → git 허브에 실제로 올리는 방법인듯

로컬서버에서 제작한 파일을 푸쉬하는법

```
git add --all
git commit -m "Initial commit"
git push -u origin main
```

루비설치 완료

루비는 깔자마자 루비전용 cmd창이 나옴.

1처음에 1번과 3번 중에 택1하라고하고, 난 1번 택했고,

마지막으로 엔터치라해서, 난 엔터침

지대로 설치되었는지 확인하려면

ruby -v 입력(루비 버전확인)

마지막으로 ird 입력

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/b30867a8-6abb-45a7-af6c-52033e167ab9/8e766cd3-5c8f-4986-acba-93b15086e46c/Untitled.png)

gem 설치 

명령어 : gem install jekyll bundler

루비가 설치된 경로를 간다음에 쳐야 함..

루비는 C드라이브에 있는데, 나는 C드라이브 \유저사용자 이런식으로 들어가서 계속 에러떳음;;

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/b30867a8-6abb-45a7-af6c-52033e167ab9/3e442bb4-6142-4a0b-94eb-1cdce765269a/Untitled.png)

명령어 : jekyll new ./

이건 클론한 내 [github.io](http://github.io/) 폴더!! 그 경로로 이동해서 쳐줘야함…

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/b30867a8-6abb-45a7-af6c-52033e167ab9/9312fb42-5caa-4151-8935-b8aeb498acda/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/b30867a8-6abb-45a7-af6c-52033e167ab9/9e5ab2ac-68b1-460c-82cb-d355503fa1a0/Untitled.png)

bundle install입력

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/b30867a8-6abb-45a7-af6c-52033e167ab9/cd69e2e2-eccb-4e5d-9d80-11ff10a9a29f/Untitled.png)

새 지킬 사이트가 C:/lunasong777.github.io에 설치되었습니다.
PS C:\[lunasong777.github.io](http://lunasong777.github.io/)> 번들 설치
번들 설치 완료! 7개의 젬 파일 종속성, 36개의 젬이 설치되었습니다.
번들 정보 [gemname]`을 사용하여 번들 젬이 설치된 위치를 확인합니다.

bundle exec jekyll serve

이 글의 제목은 {{ page.title }}이고
마지막으로 수정된 시간은 {{ page.last_modified_at }}이다.