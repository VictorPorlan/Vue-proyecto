<template>
  <div class="home" >
    <Header selected="Home"/>
    <h1>home</h1>
  </div>
</template>


<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'

export default {
  name: 'Home',
  components: {
    Header
  }
}
</script>

<style>
  .home{
    height: 100%;
  }
</style>