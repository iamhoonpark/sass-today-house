# UI

<details>
<summary>Boilerplate</summary>
<div markdown="1">

# 프로젝트 세팅

## 1. 설치 플러그인

| Plugin       | URL                                                                    |
| ------------ | ---------------------------------------------------------------------- |
| 1. 설치파일  |
| Figma        | https://www.figma.com/downloads/                                       |
| VSCode       | https://code.visualstudio.com/download                                 |
| Figma시안    | https://drive.google.com/file/d/1OJuWQ8UnZZv8GEmA5ihhqbgVBhrHoxAh/view |
| Git          | https://git-scm.com/downloads                                          |
| Git 설치방법 | https://www.youtube.com/watch?v=JKT9laOAPIs                            |

## 2. 익스텐션

- scss-lint
- Live Server
- Gitmoji
- Framer Syntax2
- Material Icon Theme

## 3. 노드설치

- Node LTS 버전
  - Long Term Support : 장기 지원 버전
  - 큰 버그 없이 무난하게 안정적으로 사용할 수 있는 버전
  - 반대로 Current Version 또는 Latest Versiont(=최신버전)
  - 따라서 Latest LTS Version(=최신 장기 지원 버전)을 권장
  - https://www.youtube.com/watch?v=AZPm7tdoQFE
  - https://www.youtube.com/watch?v=rLhPHi10uWk
- node-sass 설치
  - https://www.npmjs.com/package/node-sass
  - 옵션
    - -w: scss 실시간 코드 변경 감지
    - -r: 다중파일 감지

```sh
// 01) packge.json 파일 생성(필요한 노드모듈 다운받고 사용가능한 파일)
npm init -y

// 02) node-sass 설치(node_modules, dependencies:node-sass, package-lock.json)
npm i node-sass

// 03) (package.json)
script > "node-sass": "node-sass"

// 04) node-sass 실행
npm run node-sass

// 05) sass파일을 css파일로 변환 설정(package.json)
script > "sass": "node-sass <input> <output>"
  >  "sass": "node-sass styles/main.scss ./style.css"

// 06) 스크립트 실행(sass → css 변환)
npm run sass

// 07) 스크립트 옵션 추가(package.json)
script > "sass": "node-sass [options] <input> <output>"
  >  "sass": "node-sass -w -r styles/main.scss ./style.css"
  or  "sass": "node-sass -wr styles/main.scss ./style.css"
```

## 4. linter 설정

### 1) SCSS lint

- 일관성 있게 코드를 작성할 수 있도록 도와주는 도구
- 문법적인 실수나 정의한 규칙에 어긋날 경우 자동으로 수정(Automatic Fix)할 수 있게 함
- 익스텐션 scss-lint가 .scss-lint.yml의 규칙대로 코드가 쓰일 수 있도록 도와줌

※ Github > your gist: 코드 단위를 저장할 수 있는 곳으로 자주사용하는 설정이나 코드를 저장할 수 있음

### 2) Prittier lint

- .prettierrc 파일 생성
- VS Code Settings(ctrl + ,)
  - 검색어: format on save > Editor: Format On Save > 체크
  - 검색처: prettier config > Prettier: Require Config > 체크
- Open Setting JSON 설정
  - VS Code Settings > 문서아이콘(Open Settings)
  - "editor.defaultFormatter": "esbenp.prettier-vscode"

</div>
</details>

<details>
<summary>Asset</summary>
<div markdown="1">

# Sass

- Syntactically awesome stylesheet
- CSS Preprocessor: Sass, less, PostCss, stylus 등 CSS의 문제점들을 Programmatically 한 방식
- Sass와 SCSS는 문법의 차이며 같은 회사에서 css 전처리기로 해석되어 css로 컴파일되는 스크립트 언어
- SCSS는 Sass의 3버전에서 등장한 언어이며 퍼블리셔에게 익숙한 css와 비슷한 구문을 가지고 있으며 Sass 기능을 지원하되, css와 거의 같은 문법으로 사용된다는 점에서 퍼블리셔에게 각광받는 언어

# HTML Document 셋업

- html lang="ko" : 한국어
- meta content="width=device-width : 반응형 가능

</div>
</details>
