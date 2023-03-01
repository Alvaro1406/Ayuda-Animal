<template>
  <q-page>
    <header>
      <div class="row justify-center">
        <div class="col-12 col-sm-6 col-md-4">
          <img src="~assets/logo.png" alt="" />
        </div>
        <div class="col-12 col-sm-6 col-md-6 flex flex-center">
          <q-btn rounded falt label="Inicio" class="q-mr-md" />
          <q-btn rounded flat label="Sobre Nosotros" class="q-mr-md" />
          <q-btn rounded flat label="Lista de Animales" class="q-mr-md" />
          <q-btn rounded flat label="Contactenos" />
        </div>
      </div>
    </header>
    <div class="zona1 row flex flex-center">
      <div class="col-10">
        <h3 style="color: #26a69a">Encuentre su Mascota</h3>
        <p style="color: #000">
          Cuando ayudas o adoptas un animal estas opteniendo un pedazo de
          historia
        </p>
      </div>
    </div>
    <div class="row justify-center">
      <div class="col-10" id="phonebtn">
        <q-btn label="+53 52519414" rounded class="bg-white" />
      </div>
    </div>
    <EssentialLinkcopy />
    <EssentialLinkcopy2 />
    <EssentialLinkcopy3 />
    <EssentialLinkcopy5 />
    <EssentialLinkcopy4 />
    <EssentialLinkcopy7 />
  </q-page>
</template>

<style>
header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  justify-content: space-around;
  transition: 0.7s;
  padding: 30px 20px;
  z-index: 10;
}
.zona1 {
  position: relative;
  background-image: url(assets/7.jpg);
  width: 100%;
  height: 600px;
  background-size: cover;
  background-position: center center;
  opacity: 0.8;
}
section button {
  background-color: #fff;
}
header.abajo {
  background: #26a69a;
  padding: 5px 10px;
}
header.abajo button {
  color: #fff;
}
header img {
  width: 100px;
  height: 45px;
}
#phonebtn {
  margin-top: -20px;
}
</style>

<script setup>
import EssentialLinkcopy from "src/components/EssentialLinkcopy.vue";
import EssentialLinkcopy2 from "src/components/EssentialLinkcopy2.vue";
import EssentialLinkcopy3 from "src/components/EssentialLinkcopy3.vue";
import EssentialLinkcopy4 from "src/components/EssentialLinkcopy4.vue";
import EssentialLinkcopy5 from "src/components/EssentialLinkcopy5.vue";
import EssentialLinkcopy7 from "src/components/EssentialLinkcopy7.vue";
window.addEventListener("scroll", function () {
  var header = document.querySelector("header");
  header.classList.toggle("abajo", window.scrollY > 0);
});
</script>
