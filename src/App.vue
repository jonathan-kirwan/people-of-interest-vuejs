<template>
  <div class="container is-fluid">
    <div class="columns">
      <div class="column hero">
        <my-app-header />
      </div>
    </div>
    <main>
    <div class="columns is-multiline" id="app">
      <card v-for="item in items" 
        :key="item.id" 
        :name="item.name" 
        :phone="item.phone" 
        :avatar="item.avatar" />
    </div>
    </main>
  </div>
</template>

<script>
import headerComponent from "./components/Header.vue";
import cardComponent from "./components/Card.vue";

export default {
  name: "app",
  components: {
    "my-app-header": headerComponent,
    card: cardComponent
  },
  data() {
    return {
      items: [
        {
          id: 1,
          name: "Jon",
          phone: "07742 042 482",
          avatar: "128_1.png"
        },
        {
          id: 2,
          name: "Jen",
          phone: "07942 422 882",
          avatar: "128_6.png"
        },
        {
          id: 3,
          name: "Paul",
          phone: "07542 472 442",
          avatar: "128_2.png"
        },
        {
          id: 4,
          name: "Donna",
          phone: "08642 142 182",
          avatar: "128_4.png"
        }
      ]
    };
  }
};
</script>

<style>
#app {
  /* font-family: "Avenir", Helvetica, Arial, sans-serif; */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

body {
  background: #0f1d2e url("assets/background_pattern.png") no-repeat 0 0 /
    contain;
  font-family: "Roboto", sans-serif;
  min-height: 100vh;
}
</style>
