<template>
  <div class="root">
    <div class="row head">
      <div class="col-sm imagen">
        <img src="../assets/logo.png" style="margin-left: 50px;"/>
      </div>
      <div class="col-sm">
        <div class="buttons">
          <HeaderButton label="Home" v-bind="checkSelected('Home')" route="/" />
          <HeaderButton
            label="About"
            v-bind="checkSelected('About')"
            route="/about"
          />
        </div>
      </div>
      <div class="col-sm"></div>
    </div>
  </div>
</template>

<script>
import HeaderButton from "./HeaderButton.vue";
export default {
  name: "Header",
  props: {
    selected: String,
  },
  data() {
    return {};
  },
  components: { HeaderButton },
  methods: {
    checkSelected(nombre) {
      if (this.selected == nombre) {
        return { selected: true };
      } else {
        return { selected: false };
      }
    },
  },
};
</script>

<style>
.buttons {
  display: flex;
  justify-content: center;
}
.root {
  max-width: 100%;
  background-color: #2a2a2a;
  height: 75px;
  margin: 0px;
}
.imagen{
  text-align: start;
  align-self: center;
}
.head{
    width:100%
}
</style>