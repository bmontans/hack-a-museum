<template>
  <div>
    <vue-headful title="Contact" description="Página de contacto del museo" />
    <menucustom></menucustom>

    <!-- FORMULARIO -->
    <contactcustom></contactcustom>

    <footercustom></footercustom>
  </div>
</template>

<script>
import menucustom from "@/components/MenuCustom.vue";
import footercustom from "@/components/FooterCustom.vue";
import contactcustom from "@/components/ContactCustom.vue";

export default {
  name: "Contact",
  components: {
    menucustom,
    footercustom,
    contactcustom,
  },
};
</script>

<style scoped></style>
