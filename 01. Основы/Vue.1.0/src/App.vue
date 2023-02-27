<script>
export default {
  data() {
    return {
      visible: true
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
  <div v-if="visible">
    <p>++++</p>
    <p>++++</p>
    <p>++++</p>
  </div>
  <button @click="hide">Hide</button>
</template>

