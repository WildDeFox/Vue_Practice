<script>
export default {
  data() {
    return {
     text: '',
    };
  },
  methods: {
   
  },
};
</script>

<template>
  <p>{{ text }}</p>
  <textarea v-model="text"></textarea>
</template>

<style></style>
