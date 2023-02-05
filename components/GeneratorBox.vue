<template>
  <div class="generator-box-container">
    <h2 class="box-title">Generate Table</h2>
    <SelectorBox />
  </div>
</template>

<script>
import SelectorBox from '../components/SelectorBox.vue'

export default {
  name: 'GeneratorBox',
}
</script>

<style scoped>
  .generator-box-container {
    width: 70%;
    background-color: white;
    border-radius: 5px;
    box-shadow: 1px 1px 4px 0px rgba(0,0,0,0.25);
    padding-bottom: 20px;
    padding-top: 15px;
    margin: 30px;
  }
  .box-title {
    font-size: 20px;
    font-weight: 700;
    margin-left: 19px;
  }
</style>