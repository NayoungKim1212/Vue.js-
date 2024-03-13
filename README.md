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

## node_modules 안에 vue 패키지 존재(따로 설치한 vue도 이 안에 존재)

- 다른 패키지 설치 시 package_json dependencies, devDependencies에 추가

## vue component

- template(html)
 
- script(js)
  
- style(css)

## setup() 함수

- Vue3의 Composition API에서 사용되는 함수

   1. component 내부에서 사용
      
   2. component 데이터, 메서드 등을 정의하고 반환하는 역할

   3. 함수는 component가 생성될 때 호출되며, 컴포넌트의 초기화 작업을 수행

## Const

- 상수를 선언할 때 사용
  
  1. 한 번 할당된 값 변경 불가능

  2. 한 번 값을 할당하면 그 후에는 재할당 불가능
 
  3. 블록 범위로 제한
 
  4. 변수로 선언되고 초기화 되지 않으면 오류 발생
ex)
Const number = 3.14
number = 3; // error 발생 why? 상수라 재할당이 불가능하기 때문

## let

- 변수를 선언할 때 사용
  
  1. 변수의 값 변경 가능
 
  2. 블록 범위로 제한

  3. 변수가 선언되고 초기화 하지 않으면 undefined 설정됨
  ex)
 ```javascript
        let count = 0;
        count = 1; // 가능
````

## Var

- 재사용 가능
