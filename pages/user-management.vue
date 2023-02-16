<template>
  <div>
    <Navbar />
    <UserManagementBox />
  </div>
</template>

<script>
  import ActionButton from '~/components/ActionButton.vue';
  import Navbar from '~/components/Navbar.vue';
  import UserManagementBox from '~/components/UserManagementBox.vue';

  export default {
      name: "UserManagement",
      created() {
          //alert("Welcome")
      },
      components: { Navbar, ActionButton, UserManagementBox }
  } 
</script>