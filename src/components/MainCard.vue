<template>
  <div class="caja shadow p-3 mb-5 bg-white rounded">
    <div class="display-4 shadow p-3 bg-white rounded titulo">
      {{ title }}
    </div>
    <div class="image">
      <img src="../assets/Oficina.jpg" class="img-fluid rounded" />
    </div>
    <div class="texto">
        
          <h2 class="subtitulo">Card title</h2>
          <div class="parrafo">
          <p >
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo consequat.
          </p>
          </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
  },
};
</script>

<style>
.caja {
  background-color: white;
  border-radius: 20px;
  height: 600px;
  width: 50%;
  margin-top: 50px;
  display: grid;
  grid-template-rows: 1fr 5fr;
  grid-template-columns: 1fr 1fr;
  padding: 0px;
}
.titulo {
  grid-row: 1;
  grid-column: 1 / 3;
}
.image {
  grid-row: 2;
  grid-column: 1 / 2;
  align-self: center;
}
.texto {
  grid-row: 2;
  grid-column: 2 / 3;
  align-self: center;
  justify-content: center;
  display: grid;
  grid-template-rows: 1fr 4fr;
  height:80%
}
.subtitulo{
    grid-row: 1;
    align-self: center;
}
.parrafo{
    grid-row: 2;
    align-self: center;
    justify-self: center;
    font-size: 20px;
    width: 70%;
}
</style>