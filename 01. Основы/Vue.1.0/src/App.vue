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
  <ul>
    <template v-for="elem in hrefs">
      <li><a :href="elem.href">{{ elem.text }}</a></li>
    </template>
  </ul>
</template>
