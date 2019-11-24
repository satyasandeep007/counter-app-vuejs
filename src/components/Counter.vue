<template>
  <div id="app">
    <h2>{{counter}}</h2>
    <button v-on:click="increase">+</button>
    <button v-on:click="decrease">-</button>
  </div>
</template>

<script>
  export default {
    name : '#app',
    data() {
      return {
        counter : 0
      }
    },
    methods: {
      increase () {
        this.counter++;
      },
      decrease () {
        this.counter--;
      }
    },
  }
</script>

<style scoped>
button{
  padding: 5px;
  background-color: chocolate;
  font-weight: bolder;
}

</style>