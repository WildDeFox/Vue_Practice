<script>
export default {
  data() {
    return {
      items: [1, 2, 3, 4, 5]
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
  <div v-for="elem in items">{{ elem }}</div>
  <div v-for="elem in items">{{ elem ** 2 }}</div>
  <ul v-for="elem in items">
    <li>{{ elem }}</li>
  </ul>
</template>

