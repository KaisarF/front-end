<template>
    <div>
        <Navbar />
        <div class="form-add">
            <p class="title-form">Add New User</p>
            <form action="" class="flex flex-row flex-auto">
                <div class="w-1/2">
                    <label for="username" class="label-username">Username</label>
                    <input type="text" required name="username" id="username" placeholder="e.g john.com">
                    
                    <label for="regional" class="label-regional">Regional</label>
                    <input type="text" required name="regional" id="regional" placeholder="Input Regional">

                    <label for="status" class="label-status">Status Admin</label>
                    <div class="selectdiv">
                        <select name="status" required autocomplete="off" id="status" placeholder="Select Admin Status">
                            <option value="" selected hidden disabled class="unselect">Select Admin Status</option>
                            <option value="Web">Admin Web</option>
                            <option value="Regional">Admin Regional</option>
                            <option value="User">User</option>
                        </select>
                    </div>
                    
                    
                </div>
                
                <div class="w-1/2">
                    <label for="password" class="label-password">Password</label>
                    <input type="password" required name="password" id="password" placeholder="e.g ineedadn123">

                    <label for="confirm" class="label-confirm">Confirm Password</label>
                    <input type="password" required name="confirm" id="confirm" placeholder="e.g ineedadn123">

                    <div class="mt-9 flex flex-wrap gap-5 justify-center ">
                        <button class="cancel" type="button" @click="cancel">Cancel</button>
                        <button type="submit" class="save">Save</button>
                    </div>
                </div>
                
            </form>
        </div>
    </div>
    
</template>

<script>
  import Navbar from '~/components/Navbar.vue';
  //import Fortify from "fortify-js";


  export default {
    name: "addUser",
    data() {
      return {
        status: "Add New User",
      }
    },
    created() {
        //var field = document.getElementById('password');
        //var confirmField = document.getElementById('confirm');
        //var fortify = new Fortify(field, confirmField);
        
    }, 
    methods: {
        cancel() {
            window.location.href = '/download';
        }
    }
  } 

  
</script>

<style>

    .button-input{
        margin-top: 35px;
        display: flex;
        flex-wrap: wrap;
        gap: 22px;
        align-items: center;
        justify-content: center;
    }
    
    input, select{
        width: 95%;
        margin: 10px 10px 48px 10px;
        height: 55px;
        padding: 10px;
        box-sizing: border-box;
        background: #FFFFFF;
        border: 1px solid #7C7D80;
        border-radius: 5px;

        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 20px;
        line-height: 24px;

        
    }

    input::before, select{
        color: rgba(57, 62, 70, 0.2);
    }
    .selectdiv {
        position: relative;
    }
    .selectdiv:after {
        content: '<';
        background: #000;
        font-size: 24px;
        font-weight: bolder;
        color: rgba(57, 62, 70, 0.2);
        -webkit-transform: rotate(90deg);
        -moz-transform: rotate(90deg);
        -ms-transform: rotate(90deg);
        transform: rotate(90deg);
        right: 40px; 
        /*Adjust for position however you want*/
        
        top: 18px;
        padding: 0 0 2px;
        /*left line */
        
        position: absolute;
        pointer-events: none;
    }

    .selectdiv select{
        -webkit-appearance: none;
        -moz-appearance: none;
        appearance: none;
        /* Add some styling */
        
        line-height: 1.75;
        -ms-word-break: normal;
        word-break: normal;
    }
    option {
        color: #000000;
    }
    select::-ms-expand {
        display: none;
    }
    button {
        width: 153px;
        height: 52px;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 20px;
        line-height: 24px;
        align-items: center;
        text-align: center;

        color: #FFFFFF;
    }
    .cancel{
        background: #FF1E1E;
        box-shadow: 0px 0px 4px rgba(0, 0, 0, 0.25);
        border-radius: 5px;
    }
    .save{
        background: #2DC207;
        box-shadow: 0px 0px 4px rgba(0, 0, 0, 0.25);
        border-radius: 5px;
    }
    label {
        margin: 10px 10px 48px 10px;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 24px;
        line-height: 29px;

        color: #7C7D80;
    }
    .label-username{
        width: 100%;
    }

    #username{
        background-image: none;
    }
    .form-add {
        position: absolute;
        width: 60%;
        height: 60%;
        left: 20%;
        top: 25%;

        padding: 48px;
        background: #FFFFFF;
        box-shadow: 1px 1px 4px rgba(0, 0, 0, 0.25);
        border-radius: 5px;
    }
    .title-form {
        margin: 0px 0px 30px 0px;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 25px;
        line-height: 39px;
        display: flex;
        align-items: center;

        color: #000000;
    }
</style>