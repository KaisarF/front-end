<template>
  <button :class="childclass" @click="goto">{{ action}}</button>
</template>

<script>
export default {
  name: 'ActionButton',
  props: {
    action: String,
    childclass: String,
    link: String,
  },
  methods: {
    goto() {
      let data = this.link
      window.location.href = data;
    },
  },
}
</script>