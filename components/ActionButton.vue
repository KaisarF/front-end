<template>
  <button :class="childclass">{{ action }}</button>
</template>

<script>
export default {
  name: 'ActionButton',
  props: {
    action: String,
    childclass: String,
  }
}
</script>