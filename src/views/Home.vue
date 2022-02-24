<template>
  <div class="home" >
    <Header selected="Home"/>
    <div class="body">
      <MainCard title="Logistics"/>
    </div>
    <Footer></Footer>
  </div>
</template>


<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import MainCard from '../components/MainCard.vue'
import Footer from '../components/Footer.vue'

export default {
  name: 'Home',
  components: {
    Header,
    MainCard,
    Footer
}
}
</script>

<style>
  .body{
    height:100%;
    width: 100%;
    background-color: #BBBBBB;
    display: flex;
    justify-content: center;
    min-height:100vh;
    }
</style>