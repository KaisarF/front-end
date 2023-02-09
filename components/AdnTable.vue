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
    <tbody v-for="item in items">
      <tr>
        <td>{{ item.no }}</td>
        <td>{{ item.msisdn }}</td>
        <td>{{ item.sms }}</td>
        <td>{{ item.tanggal }}</td>
        <td>{{ item.waktu }}</td>
      </tr>
    </tbody>
  </table>
</template>

<script>
import axios from 'axios'
  export default {
    name: 'AdnTable',
    data(){
      return{
        items: []
      }
    },
    async created() {
      let getCookie = document.cookie
      let cookie = getCookie.split("Session=")
      const response = await axios.post('http://localhost:5000/api/v1/getdataadn', {
        cookies: cookie[1],
      }).catch((err) => {
        console.log(err)
      }).then((res) => {
        if (res === undefined) {
          alert("Data Not Found")
        } else {
          console.log(res.data.data)
          this.items = res.data.data
        }
      })
      
    }
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