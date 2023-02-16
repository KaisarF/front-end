<template>
  <div class="container">
    <div class="bg-white max-w-[65rem] m-6 pb-6 rounded-md shadow-md">
      <h2 class="text-xl font-bold pt-4 pl-6">Generate Table</h2>
      <hr class="ml-6 mr-8 my-2">
      <SelectorBox />
    </div>
  </div>
</template>

<script>
import SelectorBox from '../components/SelectorBox.vue'

export default {
  name: 'GeneratorBox',
}
</script>