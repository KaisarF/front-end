<template>
  <div class="input-card">
    <label class="label-title">{{ title }}</label>
    <input class="input-field" type="text" :placeholder="placeholder">
  </div>
</template>

<script>
  export default {
    name: 'InputField',
    props: {
      title: String,
      placeholder: String,
    }
  }
</script>

<style scopped>
  .label-title {
    font-weight: 700;
    font-size: 18px;
    color: #7C7D80;
    padding-bottom: 20px;
  }
  input::placeholder {
    font-weight: 700;
    font-size: 16px;
    color: rgba(57, 62, 70, 0.2);
  }
  .input-card {
    display: flex;
    flex-direction: column;
    width: auto;
    margin-left: auto;
    margin-right: auto;
    margin-top: 50px;
  }
  .label-title {
    text-align: start;
  }
  .input-field {
    width: 400px;
    height: 52px;
    border: 1px solid #7C7D80;
    border-radius: 5px;
    padding-left: 50px;
    padding-right: 50px;
  }
</style>