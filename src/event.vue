<template>
    <div class="name">
      {{ name }}
    </div>
    <button class="btn btn-primary" v-on:click="updateName">Click</button> <!---button 클릭 시 name이 updateName으로 바뀜-->
  </template>
  
  <script>
  // import {reactive} from "vue"; object or 배열은 value 사용
   import {ref} from "vue"; // vue에서 ref를 가지고 온다.
  export default { 
    setup() { // component 재사용 가능, component 내부에서만 사용 가능
      //()가 붙어있으면 함수
      
      // const name = 'Happy Corder' 
      // let name = ref('Happy Corder1')
      
      //  const name = reactive({
      //   id : 1
       const name = ref({
        id : 1
       })
  
      const updateName = () => {
         name.value.id = 2
        // name.value = 'Happy Corder' // ref는 value, object or 배열은 value 사용 X
        // name = 'Happy Corder'
      };
  
      return {
         name,
         updateName,
      };
    },
  };
  </script>
  
  <style>
  .name {
    color: red;
  }
  </style>
  <!-- -->