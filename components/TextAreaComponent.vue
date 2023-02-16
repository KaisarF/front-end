
<template>
   
    <div class="textarea-card">
      <label class="textarea-title">{{ title }}</label>
      <textarea class="textarea-field " :rows="rows"  ></textarea>
    </div>
  </template>
  
  <script>
    
    export default {
      name: 'RequestPage',
      props: {
        title: String,
        rows: String,
      }
    }
  </script>
  <style scoped>
  body{
    background-color: white;
  }
  .textarea-title {
      font-weight: 700;
      font-size: 18px;
      color: #7C7D80;
      padding-bottom: 10px;
      margin: 10px;
      width: 100%;
    }
    
    .textarea-card {
      display: flex;
      flex-direction: column;
      
    }
    .textarea-title {
      text-align: start;
    }
    .textarea-field {
      width: 93%;
      
      border: 1px solid #7C7D80;
      
      padding-left: 10px;
      padding-right: 10px;
    }
    
</style>