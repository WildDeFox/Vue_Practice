<script>
export default {
  data() {
    return {
      visible1: false,
      visible2: false,
      visible3: false,
    }
  },
  methods: {
    toggle1: function() {
      this.visible1 = !this.visible1;
    },
    toggle2: function() {
      this.visible2 = !this.visible2;
    },
    toggle3: function() {
      this.visible3 = !this.visible3;
    }


  }
}
</script>

<template>
  <div>
    <p v-if="visible1">Text1</p>
    <button @click="toggle1">Click</button>
  </div>
  <div>
    <p v-if="visible2">Text1</p>
    <button @click="toggle2">Click</button>
  </div>
  <div>
    <p v-if="visible3">Text1</p>
    <button @click="toggle3">Click</button>
  </div>
</template>

