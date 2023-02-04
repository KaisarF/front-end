<template>
  <ul class="container">
    <nuxt-link to="/" class="current-page">Download ADN</nuxt-link>
    <nuxt-link to="/">Request ADN</nuxt-link>
    <nuxt-link to="/">User Management</nuxt-link>
    <nuxt-link to="/">Exit</nuxt-link>
  </ul>
</template>

<script>
  export default {
    name: 'NavbarList',
  }
</script>

<style scoped>
  .container {
    width: 40%;
    display: flex;
    flex-direction: row;
    column-gap: 50px;
    color: white;
    justify-content: center;
    align-items: center;
    font-size: 16px;
  }
  .current-page {
    font-size: 16px;
    font-weight: 700;
  }
  a:hover {
    font-weight: bolder;
  }
</style>