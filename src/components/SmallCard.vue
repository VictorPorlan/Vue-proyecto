<template>
  <div class="cardpequeña">
      <p class="title">{{title}}</p>
      <p class="text">
        {{text}}
      </p>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    text: String
  }
}
</script>

<style>
.cardpequeña {
  background-color: white;
  border-radius: 20px;
  margin-top: 50px;
  display: flex;
  flex-direction: column;
  padding: 10px;
  width: 100%;
  align-self: center;
}
</style>