<template>
  <div>
    <vue-headful title="Roman Gallery" description="Galería de arte romano" />
    <!-- MENU -->
    <menucustom></menucustom>

    <!-- TITLE -->
    <h2>{{ title }}</h2>

    <!-- IMAGE COLLECTION -->
    <romangallery></romangallery>

    <!-- FOOTER -->
    <footercustom></footercustom>
  </div>
</template>

<script>
import menucustom from "@/components/MenuCustom";
import footercustom from "@/components/FooterCustom";
import romangallery from "@/components/RomanGallery";

export default {
  name: "RomanGallery",
  components: {
    menucustom,
    footercustom,
    romangallery,
  },
};
</script>

<style scoped></style>
