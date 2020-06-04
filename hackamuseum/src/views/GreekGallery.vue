<template>
  <div>
    <vue-headful title="Greek Gallery" description="Galería de arte griego" />
    <!-- MENU -->
    <menucustom></menucustom>

    <!-- TITLE -->
    <h2>{{ title }}</h2>

    <!-- IMAGE COLLECTION -->
    <greekgallery></greekgallery>

    <!-- FOOTER -->
    <footercustom></footercustom>
  </div>
</template>

<script>
import menucustom from "@/components/MenuCustom";
import footercustom from "@/components/FooterCustom";
import greekgallery from "@/components/GreekGallery";

export default {
  name: "GreekGallery",
  components: {
    menucustom,
    footercustom,
    greekgallery,
  },
};
</script>

<style scoped></style>
