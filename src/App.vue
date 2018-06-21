<template>
  <div class="container is-fluid has-background-info">
    <div class="columns">
      <div class="column hero">
        <header>
            <h1 class="is-size-1-mobile">
                <img src="./assets/button-bg-o.svg" style="width: 400px;" />
                <span class="is-invisible">Security Service MI5</span>
            </h1>
        </header>
      </div>
    </div>
    <div class="columns is-multiline" id="app">
        <Card name="Jon" phone="07482 424 884" avatar="128_1.png" />
        <Card name="Jen" phone="07482 424 884" avatar="128_2.png" />
        <Card name="Paul" phone="07482 424 884" avatar="128_4.png" />
        <Card name="Donna" phone="07482 424 884" avatar="128_6.png" />
    </div>
  </div>
</template>

<script>
import Card from "./components/Card.vue";

export default {
  name: "app",
  components: {
    Card
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
