<template>
  <div class="container">
    <h1 class="title">ADN DOWNLOAD MANAGER</h1>
    <div class="log-container">
      <h2>Logged in as,</h2>
      <h2>Admin Regional</h2>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'NavbarTitle',
  }
</script>

<style scoped>
  .container {
    display: flex;
    flex-direction: row;
    grid-template-columns: 3fr 1fr;
    width: 40%;
    height: 100%;
    justify-content: center;
    align-items: center;
  }
  .title {
    font-size: 20px;
    font-weight: 700;
    color: white;
  }
  .log-container {
    padding: 5px;
    border-radius: 5px;
    margin-left: 20px;
    font-size: 14px;
    font-weight: 400;
    display: flex;
    flex-direction: column;
    color: white;
    background-color: #222831;
  }
</style>
