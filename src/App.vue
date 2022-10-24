<template>
  <div>
    <h1>Hello, {{ name }}</h1>
    <h1 v-bind:class="underline">Hello</h1>
    <h1 v-bind:class="isPromoted && 'promoted'">Promoted</h1>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      name: "Luthfi",
      status: "Success",
      underline: "underlined",
      isPromoted: true
    }
  }
}
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

.underlined {
  text-decoration: underline;
}

.promoted {
    font-style: italic;
}
</style>
