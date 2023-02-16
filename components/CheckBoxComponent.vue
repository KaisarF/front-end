<template>
    <div class="Check-box">
        <input :type="type" :name="name" :value="value">
        <label :for="name">{{title}}</label><br>
    </div>
    
</template>


<script>
    export default {
      name: 'RequestPage',
      props: {
        title: String,
        name: String,
        value: String,
        type:String,
      }
    }
</script>
                                                

<style>

</style>