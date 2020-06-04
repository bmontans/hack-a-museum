<template>
  <div>
    <!-- TITLE -->
    <h2>{{title}}</h2>

    <!-- IMAGE COLLECTION -->
    <div class="estatuas">
      <div class="estatua" v-for="item in orientStatues" :key="item.id">
        <p>{{ item.name}}</p>
        <p>{{item.photographer}}</p>
        <img :src="item.urlImg" alt />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "OrientalGallery",
  data() {
    return {
      title: "COLECCIÓN ORIENTAL",
      orientStatues: [
        {
          name: "Hermenegildo III",
          photographer: "Juan Palomo",
          urlImg:
            "https://images.unsplash.com/photo-1533552755457-5b471cb2ab11?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
        },
        {
          name: "Eustaquio el Pardo",
          photographer: "Joseph Joestar",
          urlImg:
            "https://images.unsplash.com/flagged/photo-1569154707792-459d556b4bc3?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
        },
        {
          name: "Superman Veraneando",
          photographer: "Marianito el Corto",
          urlImg:
            "https://images.unsplash.com/photo-1529851494873-bd180b15801e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
        },
        {
          name: "El Jonas",
          photographer: "Andrea Andreani",
          urlImg:
            "https://images.unsplash.com/photo-1578990628004-6d50cd1afa28?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
        }
      ]
    };
  }
};
</script>

<style scoped>
</style>