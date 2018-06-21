<template>
  <div class='column is-6 has-background-primary'>
    <div class='level'>
        <div class='tile is-child is-4 has-text-centered-mobile has-text-left-tablet'>
            <img :alt="`${name} profile picture`" :src="`./assets/${avatar}`">
        </div>
        <div class='tile is-vertical is-8 is-parent has-text-centered-mobile has-text-left-tablet'>
            <header>
                <h2 class='is-size-4 is-child'>
                    <strong class='color-pink has-text-weight-semibold'>{{ name }}</strong>
                </h2>
            </header>
            <div class='tile is-child'>
                <p class='is-size-5 color-light-blue has-text-weight-semibold'>{{ phone }}</p>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    name: String,
    phone: String,
    avatar: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
