<script>
export default {
  data() {
    return {
      num: 5
    }
  },
  methods: {
  }
}
</script>

<template>
  <p v-if="num == 1">Понедельник</p>
  <p v-if="num == 2">Вторник</p>
  <p v-if="num == 3">Среда</p>
  <p v-if="num == 4">Четверг</p>
  <p v-if="num == 5">Пятница</p>
  <p v-if="num == 6">Суббота</p>
  <p v-if="num == 7">Воскресенье</p>
</template>

