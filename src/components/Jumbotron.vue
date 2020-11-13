<template>
  <b-jumbotron id="jumbot" bg-variant="info" text-variant="dark">
    <div class="text">
      <h1>HIMATIKA</h1>
      <h3 id="lead">Himpunan Mahasiswa Teknik Informatika</h3>
      <h5>UNIVERSITAS TRILOGI</h5>
    </div>
    <div v-b-hover="handleHover">
      <b-button v-if="isHovered" variant="primary" href="#"
        >Kegiatan Terbaru</b-button
      >
      <b-button v-else variant="outline-dark" class="shadow-sm rounded" href="#"
        >Kegiatan Terbaru</b-button
      >
    </div>
  </b-jumbotron>
</template>

<script>
export default {
  name: "Jumbotron",
};
</script>

<style scoped>
/* mobile */
#jumbot {
  background: url("../assets/img/bgUniv.jpg");
  background-size: cover;
  background-position: center center;
  height: 450px;
  background-attachment: fixed;
}
.text {
  color: white;
  text-shadow: 2px 2px 4px #000000;
}
.text h1 {
  font-size: 30px;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  margin-top: 80px;
}

/* dekstop */
@media (min-width: 768px) {
  #jumbot {
    background: url("../assets/img/bgUniv.jpg");
    background-size: cover;
    background-position: center center;
    height: 530px;
    background-attachment: fixed;
  }
  .text {
    color: white;
    text-shadow: 2px 2px 4px #000000;
  }

  .text h1 {
    font-size: 80px;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    margin-top: 80px;
  }
}
</style>