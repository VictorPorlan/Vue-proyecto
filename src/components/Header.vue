<template>
  <div class="root">
    <HeaderButton label="Home" v-bind="checkSelected('Home')" route="/"/>
    <HeaderButton label="About" v-bind="checkSelected('About')" route="/about"/>
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
            console.log(nombre, this.selected)
            
            if(this.selected == nombre) {
                return {selected: true}
            }
            else{
                return {selected: false}
            }
        }

    }
};
</script>

<style>
.root{
    width: 100%;
  background-color: #2a2a2a;
  height: 50px;
  display: flex;
  justify-content: center;
}
</style>