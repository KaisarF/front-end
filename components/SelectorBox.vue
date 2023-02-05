<template>
  <form class="container">
    <SelectField title="Select ADN" placeholder="Select ADN" />
    <SelectField title="Select Keyword" placeholder="Select Keyword" />
    <DateField title="Start Date" />
    <DateField title="End Date" />
    <GenerateButton />
  </form>
</template>

<script>
  import SelectField from './SelectField.vue';
  import DateField from './DateField.vue';
  import GenerateButton from './GenerateButton.vue';

  export default {
    name: "SelectorBox",
}  
</script>

<style scoped>
  .container {
    width: 100%;
    display: flex;
    flex-direction: row;
    padding-left: 5px;
    padding-right: 15px;
    align-items: flex-end;
  }
</style>