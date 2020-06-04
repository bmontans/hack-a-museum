<template>
  <div>
    <!-- MENU -->
    <menucustom></menucustom>

    <!-- TITLE -->
    <h2>{{title}}</h2>

    <!-- IMAGE COLLECTION -->
    <div class="estatuas">
      <div class="estatua" v-for="item in romanStatues" :key="item.id">
        <p>{{ item.name}}</p>
        <p>{{item.photographer}}</p>
        <img :src="item.urlImg" alt />
      </div>
    </div>

    <!-- FOOTER -->
    <footercustom></footercustom>
  </div>
</template>

<script>
export default {
  name: "RomanGallery",
  data() {
    return {
      title: "COLECCIÓN ROMANA",
      romanStatues: [
        {
          name: "Vini Vidi Vici",
          photographer: "Julito el Cesarito",
          urlImg:
            "https://images.unsplash.com/photo-1570620764320-c92b8facb70c?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
        },
        {
          name: "Bitconneeeeeeeeeeeect",
          photographer: "Jotaro Kujo",
          urlImg:
            "https://images.unsplash.com/photo-1567494472396-879c8909a768?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
        },
        {
          name: "El portal de mi casa",
          photographer: "Nero",
          urlImg:
            "https://images.unsplash.com/photo-1579449486698-0577e118ba33?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
        },
        {
          name: "Piedra",
          photographer: "The Rock",
          urlImg:
            "https://images.unsplash.com/photo-1569397906655-7a1fce6866d2?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
        }
      ]
    };
  }
};
</script>

<style scoped>
</style>