<template>
  <div class="home">
    <nav>
      navigation
    </nav>
    <h1 class="name">Griffith Asare Awuah</h1>
    <p class="description">I'm a junior software engineer and fulltime javscript merchant.</p>

    <img class="code-preview" :src="preview_img"/>
  </div>
</template>

<style scoped>
  h1.name {
    font-family: 'Fira Sans Condensed', sans-serif;
    font-size: 50px !important;
  }

  .description {
    position: relative;
    top: -20px;
    font-family: 'Fira Sans Condensed', sans-serif;
  }

</style>


<script>

export default {
  name: 'home',
  components: {

  },
  data() {
    return {
      preview_img: "./previewg.png"
    }
  }
}
</script>
