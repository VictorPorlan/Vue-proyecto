<template>
  <div class="about">
    <Header selected="About"/>
    <h1>This is an about page</h1>
    <div class="container">
      <div class="row">
        <div class="col">1 of 2</div>
        <div class="col">2 of 2</div>
      </div>
    </div>
  </div>
</template>
<script>
import Header from '@/components/Header.vue'

export default {
  name: 'About',
  components: {
    Header
  }
}
</script>
