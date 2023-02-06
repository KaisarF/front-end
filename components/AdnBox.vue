<template> 
  <div class="AdnBox">
    <AdnBar />
    <AdnTable />
    <Pagination />
  </div>
</template>

<script>
  import AdnBar from './AdnBar.vue';
  import AdnTable from './AdnTable.vue';
  import Pagination from './Pagination.vue';

  export default {
    name: "AdnBox",
    components: { AdnTable }
}
</script>

<style scoped>
  .AdnBox {
    width: 95%;
    background-color: white;
    border-radius: 5px;
    box-shadow: 1px 1px 4px 0px rgba(0,0,0,0.25);
    margin-left: 30px;
  }
</style>