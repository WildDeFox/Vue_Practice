<script>
export default {
  data() {
    return {
     checked: true,
    };
  },
  methods: {
   
  },
};
</script>

<template>
  <input type="checkbox" v-model="checked">
  <p>{{ checked ? "yes" : " " }}</p>
</template>

<style></style>
