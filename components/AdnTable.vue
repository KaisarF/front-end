<template>
  <table>
    <thead>
      <tr class="table-row">
        <th>No</th>
        <th>MSISDN</th>
        <th>SMS</th>
        <th>Tanggal</th>
        <th>Waktu</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td></td>
      </tr>
    </tbody>
  </table>
</template>

<script>
  export default {
    name: 'AdnTable',
  }
</script>

<style scoped>
  thead {
    background-color: rgba(57, 62, 70, 0.1)
  }
  .table-row {
    display: grid;
    grid-template-columns: 0.4fr 1.15fr 1.15fr 1.15fr 1.15fr;
    height: 40px;
    align-items: center;
  }
  table {
    width: 96%;
    margin-left: 30px;
  }
</style>