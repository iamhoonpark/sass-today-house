# UI

<details>
<summary>프로젝트 세팅</summary>
<div markdown="1">

## 1. 설치 플러그인
| Plugin | URL |
| ------ | ------ |
| 1. 설치파일 | 
| Figma | https://www.figma.com/downloads/ |
| VSCode | https://code.visualstudio.com/download |
| Figma시안 | https://drive.google.com/file/d/1OJuWQ8UnZZv8GEmA5ihhqbgVBhrHoxAh/view |
| Git | https://git-scm.com/downloads |
| Git 설치방법 | https://www.youtube.com/watch?v=JKT9laOAPIs |

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
</div>
</details>