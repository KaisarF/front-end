<template>
    <div class="form-request">
        <h1>ADM Request page</h1>
        <div class="form-container">
          <LeftContainerRequestPage/>
          <RightContainerRequestPage/>
      </div>

    </div>

    
    
  </template>
  
  <script>
  import LeftContainerRequestPage from './LeftContainerRequestPage.vue';
  import RightContainerRequestPage from './RightContainerRequestPage.vue';
  
    export default {
      name: 'InputField',
      components:{
        LeftContainerRequestPage,
        RightContainerRequestPage
      }
    }
  </script>
  
  <style scopped>
  body{
    background-color: #eeeeee;
    width: 100%;
  }
    .form-request{
        padding: 15px;
        
    }

  .form-container{
    display: grid;
    grid-template-columns: 1fr 1fr;
    
    background-color: white;
    padding: 30px 0px 30px 0px;
  }
  
  </style>