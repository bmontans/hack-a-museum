<template>
  <div>
    <!-- TITLE -->
    <h2>{{title}}</h2>

    <div class="estatuas">
      <div class="estatua" v-for="item in greekStatues" :key="item.id">
        <p>{{ item.name}}</p>
        <p>{{item.photographer}}</p>
        <img :src="item.urlImg" alt />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "GreekGallery",
  data() {
    return {
      title: "COLECCIÓN GRIEGA",
      greekStatues: [
        {
          name: "Hermenegildo III",
          photographer: "Juan Palomo",
          urlImg:
            "https://images.unsplash.com/photo-1549887534-1541e9326642?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
        },
        {
          name: "Eustaquio el Pardo",
          photographer: "Joseph Joestar",
          urlImg:
            "https://images.unsplash.com/photo-1506813561347-cbbdf7b3f520?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
        },
        {
          name: "Superman Veraneando",
          photographer: "Marianito el Corto",
          urlImg:
            "https://images.unsplash.com/photo-1574967197715-556d5468c1af?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
        },
        {
          name: "El Jonas",
          photographer: "Andrea Andreani",
          urlImg:
            "https://images.unsplash.com/photo-1564659907547-176f9fe0ae49?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
        }
      ]
    };
  }
};
</script>

<style scoped>
</style>