<template>
    <div class="left-container">
        <div class="first-row-left">
            <SelectComponent title="ADN Number"/>
            <InputComponent type="text" title="Keyword" placeholder="e.g SIK" />

        </div>
        <div class="second-row-left">
            <InputComponent type="text" title="Program name" placeholder="e.g SIK" />
        </div>
        <div class="third-row-left">
            <TextAreaComponent title="Program Description" rows="10" />
        </div>
        <div class="forth-row-left">
            <InputComponent type="date" title="Program Start"  />
            <InputComponent type="date" title="Program End"  />
        </div>
        <div class="fifth-row-left">
            <div class="check-box">
                <CheckBoxComponent type="checkbox" title="White List Participant" name="parent-checkbox" value="White-list" id="parent-option" v-on:onclick="activateOptions()"/>
                <div class="check-box-child" >
                    <CheckBoxComponent type="radio" title="Upload White List" name="child-checkbox1" value="upload-White-list" id="child-option-1" />
                    <CheckBoxComponent type="radio" title="WhiteList from Existing Database" name="child-checkbox2" value="White-list-from-databse" id="child-option-2"/>
                </div>
            </div>
        </div>
    </div>
        
    
</template>
<script>

import InputComponent from './InputComponent.vue';
import SelectComponent from './SelectComponent.vue';
import TextAreaComponent from './TextAreaComponent.vue';
import CheckBoxComponent from './CheckBoxComponent.vue';

export default {
    name: 'LeftContainer',
    components:{
        InputComponent,
        SelectComponent,
        TextAreaComponent,
        CheckBoxComponent
    },methods: {
       activateOptions() {
        var option1 = document.getElementById("parent-option");
        var option2 = document.getElementById("child-option-1");
        var option3 = document.getElementById("child-option-2");
            if (option1.checked == true) {
                option2.disabled = false;
                option3.disabled = false;
            } else {
                 option2.disabled = true;
                option3.disabled = true;
            }
        }
    }
  }

  
</script>
<style scoped>

.left-container{
    padding: 40px;
}

    .first-row-left{
        display: grid;
        grid-template-columns: 1fr 1fr;
        justify-self: center;
        padding-bottom: 15px;
    }
    .forth-row-left{
        display: grid;
        grid-template-columns: 1fr 1fr;
        justify-self: center;
        padding-bottom: 15px;
    }
    .second-row-left,  .third-row-left{
        padding-bottom: 15px;
    }
.check-box-child{
    padding-left: 20px;
}
   
</style>