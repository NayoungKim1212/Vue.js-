<template>
    <div class="name">
      {{ greet }} <!---변수일 때 사용 만약 함수일 경우 {{ greet() }}-->
    </div>
    <!-- <div class="name">
      {{greeting(name)}}
    </div> -->
  </template>
  
  <script>
  export default { // vue3에서만 사용 가능
    setup() { // setup 사용 시 무조건 return 미사용 시 error 발생
      const name = 'Happy Corder' // '', "" 중 아무거나 사용 가능
      const greeting = (name) => { // 화살표 함수
        return 'Hello, ' + name;
      }
  
      const greet = greeting(name);
  
      return {
        // name,
        // greeting,
        greet,
      }
    }
  }
  </script>
  
  <style>
  .name {
    color: red;
  }
  </style>