<script>
export default {
  data() {
    return {
      num: 0,
      res: 0,
      sum: 0,
      text1: '',
      text2: '',
      fio: '',
      name: '',
      surn: '',
      otx: '', 
      arr: []
    };
  },
  methods: {
    calc: function () {
      this.res = Math.sqrt(this.num);
    },
    getSum: function () {
      this.sum += Number(this.num);
    },
    clickText: function() {
      [this.text1, this.text2] = [this.text2, this.text1]
    },
    divin: function() {
      let arr = this.fio.split(' ')
      this.surn = arr[0];
      this.name = arr[1];
      this.otx = arr[2];
    }
  },
};
</script>

<template>
  <div>
    <button @click="calc">Квадратный корень</button>
    <button @click="getSum">Сумма</button>
    <input type="text" v-model="num" />
    <p>Квадратный корень: {{ res }}</p>
    <p>Сумма: {{ sum }}</p>
  </div>

  <div>
    <input type="text" v-model="text1" />
    <input type="text" v-model="text2" />
    <button @click="clickText">Click me!</button>
  </div>
  <div>
    <input type="text" v-model="fio">
    <button @click="divin">Разделить</button>
    <p>Фамилия: {{ surn }}</p>
    <p>Имя: {{ name }}</p>
    <p>Отчество: {{ otx }}</p>
  </div>
</template>

<style></style>
