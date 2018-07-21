<template>
  <div class="home">
    <navigation/>

    <h1 class="name">Griffith Asare Awuah</h1>
    <p class="description">I'm a junior software engineer, product designer and fulltime javscript merchant.</p>
    <p class="current-position">Currently work as a fullstack intern at <a class="aidahbot-text" href="https://www.aidahbot.com">Aidahbot Company</a></p>
    <p class="spread-love">...</p>


    <img class="code-preview" :src="preview_img"/>

    <div class="cards-container">

    </div>
  </div>
</template>

<style scoped>
  .home{
    /* border: 1px solid green; */
    height: 100vh;
    box-sizing: border-box;
    font-family: 'Fira Sans Condensed', sans-serif;
    /* background: url(../../public/avatar.jpeg);
    background-repeat: no-repeat;
    background-size: cover; */
  }

  h1.name {
    font-size: 60px !important;
  }

  .description {
    margin-top: -34px;
    font-size: 20px;
  }

  .current-position, .spread-love {
    margin-top: -10px;
    font-size: 18px;
  }

  .current-position .aidahbot-text {
    text-decoration: none;
  }

</style>


<script>

import Navigation from '@/components/Navigation'

export default {
  name: 'home',
  components: {
    Navigation
  },
  data() {
    return {
      preview_img: "./previewg.png"
    }
  }
}
</script>
