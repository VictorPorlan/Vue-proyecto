<template>
  <router-link
    v-bind:to="route"
    class="root"
    style="text-decoration: none;"
  >
    <div class="text">
      {{ label }}
    </div>
    <div class="selected" v-if="selected"></div>
  </router-link>
</template>

<script>
export default {
  name: "HeaderButton",
  props: {
    label: String,
    selected: Boolean,
    route: String
  },
  data() {
    return {};
  },
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
.root {
  background-color: #2a2a2a;
  color: #ffffff;
  width: 100px;
  height: 50px;
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 1fr 1fr 1fr;
}
.text {
  grid-row: 2;
}
.selected {
  background-color: #ffffff;
  height: 5px;
  width: 80%;
  grid-row: 3;
  align-self: flex-end;
  margin-left: auto;
  margin-right: auto;
}
</style>
