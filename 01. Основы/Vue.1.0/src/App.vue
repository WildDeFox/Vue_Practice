<script>
export default {
  data() {
    return {
      text: "",
      pageText: "",
      linkText: "",
    };
  },
  methods: {
    clickEnter: function () {
      this.pageText = this.text;
    },
    clikcLinkLeft: function () {
      this.linkText = "Левая кнопка мыши";
    },
    clickLinkRight: function () {
      this.linkText = "Правая кнопка мыши";
    },
    clickLinkMidle: function () {
      this.linkText = "Средняя кнопка мыши";
    }
  },
};
</script>

<template>
  <input type="text" v-model="text" @keyup.enter="clickEnter" />
  <p>{{ pageText }}</p>
  <a href="#" @click.prevent @click.ctrl.left="clikcLinkLeft" @click.ctrl.right="clickLinkRight" @click.ctrl.middle="clickLinkMidle">Ссылка</a>
  <p>{{ linkText }}</p>
</template>
