
import UsernameInput from './UsernameInput.vue';

<template>
  <form class="card">
    <InputField title="Username" placeholder="e.g. john.com" />
    <InputField title="Password" placeholder="e.g. ineedadn123"/>
    <SignInButton />
  </form>
</template>

<script>
import InputField from './InputField.vue';
import SignInButton from './SignInButton.vue';

export default {
  name: 'Form',
}
</script>

<style>
  .card {
    display: flex;
    width: 550px;
    height: 450px;
    flex-direction: column;
    background-color: white;
    margin: auto;
    margin-top: 120px;
    border-radius: 8px;
    box-shadow: 1px 1px 4px 0px rgba(0,0,0,0.25);
    -webkit-box-shadow: 1px 1px 4px 0px rgba(0,0,0,0.25);
    -moz-box-shadow: 1px 1px 4px 0px rgba(0,0,0,0.25);
  }
</style>
