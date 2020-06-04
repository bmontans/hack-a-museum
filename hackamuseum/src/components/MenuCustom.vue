<template>
  <div>
    <div id="nav">
      <router-link :to="{name: 'Home'}">Home</router-link>|
      <router-link :to="{name: 'Contact'}">Contact</router-link>
      <br />
    </div>
    <div id="gallery">
      <router-link :to="{name: 'GreekGallery'}">Greek Gallery</router-link>|
      <router-link :to="{name: 'OrientalGallery'}">Oriental Gallery</router-link>|
      <router-link :to="{name: 'RomanGallery'}">Roman Gallery</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "MenuCustom"
};
</script>


<style scoped>
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
  padding: 1rem;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

#gallery a {
  font-weight: bold;
  color: #2c3e50;
  padding: 1rem;
}

#gallery a.router-link-exact-active {
  color: #42b983;
}
</style>
