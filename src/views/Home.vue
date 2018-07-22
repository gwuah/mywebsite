<template>
  <div class="home">
    <navigation class="navigation"/>

    <h1 class="name">Griffith Asare Awuah</h1>
    <p class="description">I'm a junior software engineer, aspiring product designer and fulltime javscript merchant.</p>
    <p class="current-position">Currently working as a fullstack intern at <a class="aidahbot-text" href="https://www.aidahbot.com">Aidahbot Company</a></p>
    <p class="spread-love">...</p>


    <!-- <img class="code-preview" :src="preview_img"/> -->

    <div class="skills-container">
      <skill-tablet v-for="(skillset, key) in skills" :skill="skillset.skill" :key="key" :color="skillset.color"/>
    </div>

    <div class="mini-contact">
      Do I look like your guy? If yes, then let's talk. 
      <a href="https://twitter.com/gwuah_"><i data-feather="twitter"></i></a>
      <a href="https://www.linkedin.com/in/griffith-awuah-b00a62112/_"><i data-feather="linkedin"></i></a>
      <a href="https://facebook.com/gwuah_"><i data-feather="facebook"></i></a>
      <a href="https://github.com/gwuah_"><i data-feather="github"></i></a>
    </div>

  </div>
</template>

<style scoped>
  .navigation {
    margin-bottom: 150px;
  }

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

  .skills-container {
    /* margin-top: -30px; */
    padding: 10px;
    width: 60%;
    margin: 0 auto;
    border: 1px solid #f1f1f1;
    display: flex;
    justify-content: space-around
  }

  .mini-contact {
    width: 60%;
    margin: 0 auto;
    line-height: 80px;
    margin-top: 25px !important;
    border: 1px solid red;
  }

  .mini-contact svg {
    margin: 10px;
  }

</style>


<script>

import Navigation from '@/components/Navigation';
import SkillTablet from '@/components/SkillTablet';

export default {
  name: 'home',
  components: {
    Navigation,
    SkillTablet
  },
  data() {
    return {
      preview_img: "./previewg.png",
      skills: [
        {skill:"reactjs", color: " #f1f1f1"},
        {skill:"vuejs", color: null},
        {skill:"html", color: null},
        {skill:"css", color: null},
        {skill:"es5/es6/es7", color: null},
        {skill:"typescript", color: null},
        {skill:"jquery", color: null},
        {skill:"nodejs", color: null},
        {skill:"express", color: null},
        {skill:"scss", color: "#f1f1f1"},
        {skill:"python", color: null},
        {skill:"git", color: null},
        {skill:"postgres", color: "#f1f1f1"},
        {skill:"graphql", color: "#f1f1f1"}
      ]
    }
  },
  mounted() {
    // feather ? feather.replace() : alert("there's no feather")
    // eslint-disable-next-line
    feather.replace()
  }
}
</script>
