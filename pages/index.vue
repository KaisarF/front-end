<template>
  <div id="app">
    <LoginTitle />
    <Form />
    <img class="vector1" src="../assets/image/vector1.png" alt="vector">
    <img class="vector2" src="../assets/image/vector2.png" alt="vector2">
  </div>
  
</template>

<script>
import Form from '../components/Form.vue'
import LoginTitle from '../components/LoginTitle.vue';

export default {
    name: "IndexPage",
}
</script>

<style scoped>
  .vector1 {
    position: absolute;
    top: 120px;
    right: 300px;
    z-index: -1;
    width: 250px;
  }
  .vector2 {
    position: absolute;
    bottom: 50px;
    left: 250px;
    z-index: -1;
    width: 100px;
  }
</style>
