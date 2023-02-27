<script>
export default {
  data() {
    return {
      isAdmin: true
    }
  },
  methods: {
  }
}
</script>

<template>
  <p v-if="isAdmin">Вы админ</p>
  <p v-else>Вы не админ</p>
</template>

