<template>
    <div class="right-container">
        <div class="first-row-right">
            <SelectComponent title="ADN Type"/>
            <SelectComponent title="ADN Price"/>
        </div>
        <div class="second-row-right">
            <TextAreaComponent title="SMS Replay Succes" rows="8" />
        </div>
        <div class="third-row-right">
            <TextAreaComponent title="SMS Replay Reject" rows="8" />
        </div>
        <div class="forth-row-right">
            
            <div id="input-area">
                <InputComponent type="text" title="Data Label" placeholder="e.g SIK" />
                <div >
                    <ActionButton childclass="bg-green-500 w-10 h-10 rounded"  />
                </div>
                
            </div>
            
        </div>
        
    </div>

    
</template>
<script>
import InputComponent from './InputComponent.vue';
import SelectComponent from './SelectComponent.vue';
import TextAreaComponent from './TextAreaComponent.vue';
import ActionButton from './ActionButton.vue';

export default {
    name: 'RightContainer',
    components:{
        InputComponent,
        SelectComponent,
        TextAreaComponent,
        ActionButton
    }
  }
</script>
<style scoped>
.right-container{
    padding: 40px;
}

    .first-row-right{
        display: grid;
        grid-template-columns: 1fr 1fr;
        padding-bottom: 15px;
    }
    .third-row-right, .second-row-right{
    padding-bottom: 15px;
}

    #input-area{
        display: grid;
        grid-template-columns: 6fr 1fr
    }
    .label-forth-row-right {
      font-weight: 700;
      font-size: 18px;
      color: #7C7D80;
      padding-bottom: 10px;
      margin: 10px;
      width: 100%;
    }
.add-button{
    color: chartreuse;
}

</style>