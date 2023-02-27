<script>
export default {
  data() {
    return {
      arr: ['x', 'y', 'z']
    }
  },
  methods: {
    hide: function() {
      this.visible = !this.visible
    }
  }
}
</script>

<template>
  <ul v-for="(elem, key) in arr">
    <li>{{ key }}</li>
  </ul>
</template>

