<template>
  <div class="input-card">
    <label class="label-title">{{ title }}</label>
    <select class="input-field" placeholder="apa">
      <option class="placeholder" value="" disabled selected>{{ placeholder }}</option>
      <option></option>
      <option></option>
      <option></option>
    </select>
      <!-- <option :value={{ value.name }}>{{ value.name }}</option> -->
  </div>
</template>

<script>
export default {
  name: 'SelectField',
  props: {
    title: String,
    placeholder: String,
    values: ['apa'],
  } 
}
</script>

<style scoped>
.label-title {
  font-weight: 700;
  font-size: 16px;
  color: #7C7D80;
  padding-bottom: 5px;
}
input:placeholder {
  font-weight: 700;
  font-size: 12px;
  color: rgba(57, 62, 70, 0.2);
}
.input-card {
  display: grid;
  flex-direction: column;
  width: auto;
  margin-left: auto;
  margin-right: auto;
  margin-top: 10px;
}
.label-title {
  text-align: start;
}
.input-field {
  width: 200px;
  height: 40px;
  border: 1px solid #7C7D80;
  border-radius: 5px;
  padding-left: 10px;
  padding-right: 10px;
}
</style>