<template>
  <div class="hello">
    <div class="wallpaper">
      <!-- <img 
      :src="wallpaper.image" 
      :alt="wallpaper.alt"> -->
    </div>
    <h1>{{ msg }}</h1>
  </div>

</template>

<script>

export default {
  name: 'HelloWorld',
  data: () => ({
    wallpaper: {
      image: 'images/img.png',
      alt: 'Background-image'
    }
  }),
  props: {
    msg: String,
  }
}
</script>

<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.wallpaper {
  max-height: 10%;
}
.wallpaper:empty {
  background: gray;
}
.wallpaper > img {
  max-width: 100%;
  height: auto;
}

</style>
