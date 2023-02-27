<script>
export default {
  data() {
    return {
      cost: 154,
      amount: 1
    }
  },
  methods: {
   change: function() {
    this.amount++
   }
  },
  computed: {
    price: function() {
      return this.cost * this.amount;
    }
  }
}
</script>

<template>
  <div>{{ price }}</div>
  <button @click="change()">Ещё один!</button>
  <a @click.prevent href="google.com">Link</a>
</template>

