<script>
import axios from 'axios';


export default {
    name: "AddUser",
    async created() {
        //var field = document.getElementById('password');
        //var confirmField = document.getElementById('confirm');
        //var fortify = new Fortify(field, confirmField);
        let getCookie = document.cookie
        let cookie = getCookie.split("Session=")
        let ulrParams = new URLSearchParams(window.location.search)

        await axios.post('http://localhost:5000/api/v1/deleteuser', {
            cookies: cookie[1],
            id : ulrParams.get('id'),
        }).catch((err) => {
            console.log(err)
        }).then((res) => {
            if (res === undefined) {
                alert("Incorrect Id - "+ulrParams.get('id')+"!!")
            } else{
                if (res.status == 200) {
                    window.location.href = '/user-management';
                }
            }
        })
    }, 
}
</script>