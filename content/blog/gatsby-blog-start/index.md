---
title: Gatsby 블로그 시작!
date: "2024-01-11T01:27:26.322Z"
---

예전부터 블로그를 만들고자 했는데, 드디어 만들었다. 블로그를 통해서 머릿속에 숨어있는 내 생각을 머리 밖으로 꺼내고자하는 욕구, 생각의 꼬리의 꼬리를 이어나가면서 사고 과정을 기록하고 싶은 욕구는 항상 있었다. 또한 작년부터 제대로된 '일' 이라는 것을 하게 되면서 많이들 얘기하는 `기록하는 것`의 중요성은 많이 들은 것을 넘어서서 격하게 체감하고 있었다. 

이와 관련된 이야기는 따로 적는걸로 하고, 일단 이렇게 나만의 블로그를 만들게되어서 뿌듯하다. 이 역사적인 블로그 생성에 가장 큰 동기부여를 해주신 **덕수님**께 감사하다는 말씀드리며, 앞으로 내 개인적인 생각과 개발, 비즈니스 관련(혹은 다른 관심있는 분야 관련) 지식들을 꾸준히 채워나갈 예정이다.

## Gatsby란?
- 웹사이트를 만들기 위한 React-based 오픈 소스 프레임워크
- 다양한 Gatsby blog 템플릿을 [홈페이지](https://www.gatsbyjs.com/starters/)에서 제공하고 있다.

## 블로그 배포
- github pages를 통해 배포할 예정.

## 기본 세팅
0. {github_id}.github.io 라는 repository 생성
1. `gatsby-cli` 설치
`npm install -g gatsby-cli`

2. 원하는 폴더에 `my-gatsby-project` 라는 gatsby project 생성
`gatsby new my-gatsby-project https://github.com/gatsbyjs/gatsby-starter-blog`

3. `npm run start` -> localhost:8000에서 웹사이트 확인 가능

4.  `my-gatsby-project` 로 가서 해당 폴더의 git 초기화 후, 미리 만들어놓은 {github_id}.github.io repository에 연결
```
rm -rf .git
git init
git add .
git commit -m "Init blog project"
git branch -M main
git remote add origin https://github.com/psong0808/psong.github.io.git
git push -u origin main
```

5. repository의 `Settings` -> `Pages`에서 Build and deployment branch를 `gh-pages`로 설정
6. `gh-pages` branch로 public 폴더 배포하기
- 특정 브랜치에 index.html 이 존재하면 정적 페이지 배포가 가능하다.
- 브랜치를 생성해서 index.html 을 push 하면 된다.
	- `npm run build`를 통해 build된 파일들이 /public 폴더에 생기고, 이 /public 폴더를 `gh-pages` 브랜치에 push

## 앞으로 배울 것
- gatsby-browser.js, gatsby-config.js, gatsby-ssr.js 등 gatsby의 다양한 기능에 대해서 차근차근 공부할 필요가 있어보임.
- [Gatsby tutorial 페이지](https://www.gatsbyjs.com/docs/tutorial/getting-started/)

## 앞으로 해야할 것
- CSS customize
- Google Search Console, Google Analytics 연결
 
> 시작이 반이다... 이제부턴 꾸준히 적어보자!