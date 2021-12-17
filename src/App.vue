<template>
  <Card />
  <Copyright />
</template>

<script>
import Card from './components/Card.vue'
import Copyright from './components/Copyright.vue'

export default {
  name: 'App',
  components: {
    Card,
    Copyright,
  },
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: $dark-blue-1;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100vh;
}
</style>
