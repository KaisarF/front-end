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
// text-base font-semibold text-white py-3 px-8 rounded-lg w-10 hover:opacity-80 hover:shadow-lg transition duration-500 bg-red
</script>