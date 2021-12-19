<template>
  <div class="container">
    <Card />
    <Copyright />
  </div>
</template>

<script>
import Card from './components/Card.vue';
import Copyright from './components/Copyright.vue';

export default {
  name: 'App',
  components: {
    Card,
    Copyright,
  },
};
</script>

<style lang="scss">
@import './styles/normalize.scss';

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  background-color: $dark-blue-1;
  display: flex;
  justify-content: space-evenly;
  flex-direction: column;
  align-items: center;
  width: 100%;
  min-height: 100vh;
}
</style>
