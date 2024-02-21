<template>
  <div class="name">
    {{ name }}
  </div>
  <!-- <input type="text" :value="name" @input="updateName"> -->
  <input type="text" v-model="name"> 
  <button class="btn btn-primary" @click="onSubmit">Click</button> 
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    const name = ref('Happy')

    
    const onSubmit = () => {
      console.log(name.value)

    };

    // const updateName = (e) => {
    //   console.log(e.target.value)
    //   name.value = e.target.value;

    // };

    return {
      name,
      onSubmit,
    //  updateName,
    };
  },
};
</script>

<style>
.name {
  color: red;
}
</style>
<!--양방향 바인딩-->