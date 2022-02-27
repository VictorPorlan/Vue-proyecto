<template>
  <div class="cards-root">
    <div class="card" style="width: 18rem">
      <img
        class="card-img-top"
        src="../assets/Oficina.jpg"
        alt="Card image cap"
      />
      <div class="card-body">
        <h5 class="card-title">Equipamiento</h5>
        <p class="card-text">
          Disponemos del mejor equipo a la hora de programar para que tu código
          pueda ser lo más eficiente posible
        </p>
        <a href="#" class="btn btn-primary">Saber más</a>
      </div>
    </div>
    <div class="card" style="width: 18rem">
      <img
        class="card-img-top"
        src="../assets/oficina2.jpg"
        alt="Card image cap"
        style="height: 245px"
      />
      <div class="card-body">
        <h5 class="card-title">Compañeros</h5>
        <p class="card-text">
          Los mejores programadores de la zona estarán a tu disposición para
          ayudarte en lo que necesites siempre.
        </p>
        <a href="#" class="btn btn-primary">Saber más</a>
      </div>
    </div>
    <div class="card" style="width: 18rem">
      <img
        class="card-img-top"
        src="../assets/oficina3.jpg"
        alt="Card image cap"
        style="height: 245px"
      />
      <div class="card-body">
        <h5 class="card-title">Instalaciones</h5>
        <p class="card-text">
          Instalaciones de última generación, con un estilo minimalista y
          calmado para la máxima concentración en tu trabajo.
        </p>
        <a href="#" class="btn btn-primary">Go somewhere</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.cards-root {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width: 60%;
}
@media only screen and (max-width: 1200px) {
  .cards-root {
    flex-direction: column;
    align-items: center;
  }
  .card {
    margin-top: 10px;
  }
}
</style>