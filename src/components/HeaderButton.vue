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
@import url('https://fonts.googleapis.com/css2?family=Barlow:wght@300&display=swap');

@keyframes createBox {
  from {
    transform: scale(0);
  }
  to {
    transform: scale(1);
  }
}
.root {
  background-color: #2a2a2a;
  color: #ffffff;
  width: 100px;
  height:75px;
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 1fr 1fr 1fr;
}
.text {
  grid-row: 2;
  font-family: "Barlow";
}
.selected {
  animation: createBox .25s;
  background-color: #ffffff;
  height: 3px;
  width: 60%;
  margin-bottom: 10px;
  grid-row: 3;
  align-self: flex-end;
  margin-left: auto;
  margin-right: auto;
}
</style>
