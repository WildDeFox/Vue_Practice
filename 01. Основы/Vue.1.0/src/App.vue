<script>
export default {
  data() {
    return {
      visible: false,
    }
  },
  methods: {
    click: function() {
      this.visible = true
    },

    hide: function() {
      this.visible = false
    }
  }
}
</script>

<template>
  <p v-if="visible">Hello World!</p>
  <button v-if="!visible" @click="click">Показать</button>
  <button v-if="visible" @click="hide">Скрыть</button>
</template>

