<template>
  <div id="app">
    <input type="number" v-model="person" />
    <button @click="shoPerson()">Click me</button>
    <TestProp msg="test"></TestProp>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import TestProp from './components/TestProp.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
  },
  data: function () {
    return {
      person: '20',
    };
  },
  methods: {
    shoPerson() {
      alert(this.person);
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
