<script>
export default {
  data() {
    return {
      hrefs: [
        { href: "1.html", text: "text1" },
        { href: "2.html", text: "text2" },
        { href: "3.html", text: "text3" },
      ],
    };
  },
};
</script>

<template>
  <p v-for="num in 30">{{ num }}</p>
</template>
