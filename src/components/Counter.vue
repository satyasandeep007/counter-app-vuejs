<template>
  <div id="app">
    <h1>
      Counter :
      <span class="badge badge-secondary">{{counter}}</span>
    </h1>
    <button v-on:click="increase" type="button" class="btn btn-success">Add</button>
    <button v-on:click="reset" type="button" class="btn btn-primary">Reset</button>
    <button v-on:click="decrease" type="button" class="btn btn-danger">Subtract</button>
  </div>
</template>

<script>
export default {
  name: "#app",
  data() {
    return {
      counter: 0
    };
  },
  methods: {
    increase() {
      this.counter++;
    },
    decrease() {
      this.counter--;
    },
    reset() {
      this.counter = 0;
    }
  }
};
</script>

<style scoped>
#app{
  margin: 15% auto;
  margin-left: 40%;
}
button{
  margin-top: 10px;
  margin-right: 7px;
}
</style>