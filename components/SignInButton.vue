<template>
  <button type="submit" class="signin-button">Sign In</button>
</template>

<script>
  export default {
    name: 'SignInButton',
  }
</script>

<style scoped>
  .signin-button {
    background: linear-gradient(45deg, rgba(34,40,49,1) 0%, rgba(34,40,49,0.9080882352941176) 71%, rgba(34,40,49,0.7792366946778712) 91%, rgba(34,40,49,0.6896008403361344) 100%);
    font-weight: 800;
    font-size: 18px;
    color: white;
    border-radius: 200px;
    width: 300px;
    height: 52px;
    margin-top: 50px;
    margin-left: auto;
    margin-right: auto;
  }
  .signin-button:hover {
    background: linear-gradient(45deg, rgba(34,40,49,1) 0%, rgba(34,40,49,0.9080882352941176) 37%, rgba(34,40,49,0.7792366946778712) 68%, rgba(34,40,49,0.6896008403361344) 100%);
  }
</style>