<template>
  <div class="home">
    <vue-headful title="Hack a Museum" description="Hack a Museum" />
    <!-- MENU -->
    <menucustom></menucustom>

    <!-- TITLE -->
    <h2 v-html="title"></h2>

    <!-- VIDEO -->
    <iframe
      width="1280"
      height="720"
      src="https://www.youtube.com/embed/6vuFh6NNa70"
      frameborder="0"
      allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
    ></iframe>

    <!-- DESCRIPTION -->
    <p v-html="desc"></p>

    <!-- FOOTER -->
    <footercustom></footercustom>
  </div>
</template>

<script>
import menucustom from "@/components/MenuCustom.vue";
import footercustom from "@/components/FooterCustom.vue";

export default {
  name: "Home",
  components: {
    // REGISTRANDO EL COMPONENTE
    menucustom,
    footercustom,
  },
  data() {
    return {
      title: "Te damos la bienvenida <br> a HACK A MUSEUM",
      desc:
        "Tenemos varias colecciones de arte que te pueden interesar, <br> y buscamos colaboradores/as activamente.",
    };
  },
};
</script>

<style></style>
