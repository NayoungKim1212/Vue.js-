<template>
  <div :class="nameClass">
    {{ name }}
  </div>
  <input :type="type" :value="name"> 
  <!---속성은 다 bind 가능, v-bind:속성값 => :속성값으로 축약 가능-->
  <button class="btn btn-primary" @click="updateName">Click</button> 
  <!--v-onclick => @로 축약 가능-->
</template>

<script>
import { ref } from "vue";
export default {
  setup() {
    const name = ref('Happy')
    const type = ref('number')
    const nameClass = ref('name') // name을 지워주면 style의 color 변경 X

    const updateName = () => {
      name.value = 'Corder'
      type.value = 'text'
    };

    return {
      name,
      updateName,
      type,
      nameClass,
    };
  },
};
</script>

<style>
.name {
  color: red;
}
</style>