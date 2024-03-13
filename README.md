# Vue.js

## Vue.js 방식 2가지

### 1. CDN 방식

- HTML 파일에 <script> 태그를 추가함으로써 Vue.js를 직접 포함시키는 방법

### 2. NPM 방식

- CLI를 통해 설치하면 node.js도 같이 설치되서 자동으로 사용이 가능

## 개발 환경을 설정하고 관리하기 위한 도구

### 1. CLI

-  Vue.js 프로젝트를 생성하고 구성하기 위한 공식 커맨드 라인 인터페이스로 node.js와 같이 사용

-  프로젝트의 초기 설정, 개발, 빌드 및 배포 과정을 단순화함

  #### 1.1 설치 명령어

  ##### 1) npm의 경우
>npm install -g @vue/cli

  ##### 2) yarn의 경우
>yarn global add @vue/cli

### 2. Vite

- Vue CLI를 대체하기 위한 툴로 내 로컬에서만 사용 가능

- Vue.js를 포함한 여러 프론트엔드 프레임워크와 함께 사용

- 빠른 콜드 스타트, 즉각적인 모듈 리로딩, 그리고 빌드 최적화를 제공하여 개발자의 생산성을 높여줌

  #### 1.1 Vite 기반의 Vue 프로젝트 생성
  >$ npm create vite@latest
