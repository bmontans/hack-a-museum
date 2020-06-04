<template>
  <div>
    <vue-headful
      title="Oriental Gallery"
      description="Galería de arte oriental"
    />
    <!-- MENU -->
    <menucustom></menucustom>

    <!-- TITLE -->
    <h2>{{ title }}</h2>

    <!-- IMAGE COLLECTION -->
    <orientalGallery></orientalGallery>

    <!-- FOOTER -->
    <footercustom></footercustom>
  </div>
</template>

<script>
import menucustom from "@/components/MenuCustom";
import footercustom from "@/components/FooterCustom";
import orientalGallery from "@/components/OrientalGallery";

export default {
  name: "OrientalGallery",
  components: {
    menucustom,
    footercustom,
    orientalGallery,
  },
};
</script>

<style scoped></style>
