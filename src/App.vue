<template>
  <div>
    <input v-model="name" type="text" />
    {{ name }}
    <hr />
    <button @click="incrementCounter">Add To increment</button>
    {{ counter }}
  </div>
</template>
<script>
export default {
  data() {
    return {
      name: "sofien",
      counter: 0,
    };
  },
  methods: {
    incrementCounter() {
      this.counter++;
    },
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
