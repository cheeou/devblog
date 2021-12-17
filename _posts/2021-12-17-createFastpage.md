---
toc: true
layout: post
description: fastpage로 깃허브 블로그 만드는 방법
categories: [github vlog]
title: # github vlog 초간단 깃허브 블로그 만들기💫
---


## ⚡️ fastpages로 최단시간으로 깃허브 블로그 만들기

`fastpages`는 Github Action [^1]으로 간단하게 Jeklly blog 포스팅을 할 수있게 도와준다.<br/>

드디어 지킬 블로그에서 겪은 좌절을 fastpages로 치유했다!! (-_-)b

![image](https://user-images.githubusercontent.com/77304817/146552499-cd21082c-5807-44ca-8e82-f38a554bf506.png)



<br/>

## 🔮블로그 생성하기


1. https://github.com/fastai/fastpages url에 접속 후 `README.md`에서 `Setup Instructions` 목차링크를 클릭한다. <br/>


2. 해당 내용에 `on this link`를 링크를 클릭하여 https://github.com/fastai/fastpages/generate url로 이동하여 저장소를 생성한다. <br/>
  📌참고로 fastpage에서 생성한 블로그 url은  https://[github계정이름].github.io/[저장소이름]/ 형식이다.<br/>
  
3. 생성한 저장소에서 상단에 `Pull requests` 탭에 일정 시간이 지나면(약 3분이내)`Initial Setup`이 하나 업데이트 되어있을 것이다. <br/>
  `Before you merge this PR` 내용에 순서대로 셋업을 진행한다. ‼️링크 이동할 때는 새창으로 열어주세요.
     - `Before you merge this PR` 1번 내용에 `this utility` 링크를 클릭 후 `Generate SSH Keys Online` 페이지로 이동한다. <br/>
     - SSH-Keygen Oline : RSA | RSA Key Size : 4096 체크를 하면 자동으로 PrivateKey와 Public key가 발행된다. <br/>우선 `PrivateKey` 내용을 전부 복사 후,<br/>
      `Before you merge this PR` 2번 내용에 `this link` 링크를 클릭 후 오른쪽 상단에 `New repository secret`을 클릭 후, 시크릿 키 `Name`을 입력하고 (ex. SSH_DEPLOY_KEY) `Value`에 복사한 `PrivateKey`를 붙여 넣고 `Add secret`으로 등록한다.
     - `Before you merge this PR` 3번 내용에 `this link` 링크를 클릭 후 이번엔 `Public key` 내용을 전부 복사하고 `Add deploy key`를 눌러 원하는 블로그 타이틀을 `Title`에 적고, `Key`에  `Public key`내용을 붙여넣고 ✅Allow write access 체크 후 `Add key`로 등록한다.<br/>
     
4. 다시 해당 github 저장소로 돌아가서 `Pull requests` 탭에 `Initial Setup` 클릭 후 스크롤을 내려 `Merge pull request` 클릭 후-> `Confirm merge` 를 눌러주면 끝!<br/>
   해당 요청이 완료될 때까지 2분정도 소요가 된다. 처리 상태를 보고 싶다면 상단에 `Actions`탭에서 진행사항 확인이 가능하다.
     
     
## 🔮Hit Tracker 만들기
## 🔮Github 잔디 심기



## Footnotes



[^1]: Github 저장소 기반으로 software 개발 Workflow를 자동화 할 수 있는 도구.
