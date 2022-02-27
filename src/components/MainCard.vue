<template>
  <div class="caja shadow p-3 mb-5 bg-white rounded">
    <div class="display-4 shadow p-3 bg-white rounded titulo">
      {{ title }}
    </div>
    <div class="image">
      <img
        src="../assets/oficinista.jpg"
        class="rounded mx-auto d-block"
        style="width: 90%"
      />
    </div>
    <div class="texto">
      <h1 class="subtitulo">Bienvenido</h1>
      <div class="parrafo">
        <p>
          En esta empresa apostamos por la comodidad y la eficiencia de nuestros
          empleados, para conseguirlo, optamos por los diseños más modernos y
          actualizados en nuestras instalaciones, máquinas perfectamente
          preparadas para su uso y un ambiente de trabajo totalmente libre de
          estrés y con gran apoyo de tus compañeros.
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
  width: 60%;
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
  height: 60%;
}
.subtitulo {
  grid-row: 1;
  align-self: center;
}
.parrafo {
  grid-row: 2;
  justify-self: center;
  align-self: center;
  font-size: 20px;
  width: 80%;
}
@media only screen and (max-width: 1200px) {
  .caja {
    width: 90%;
    grid-template-rows: 1fr 3fr 5fr;
    grid-template-columns: 1fr;
  }
  .texto {
    grid-row: 3;
    grid-column: 1;
    align-self: flex-start;
    justify-content: center;
  }
  .image {
    grid-row: 2;
    grid-column: 1;
    margin-top: 20px;
  }
}
</style>