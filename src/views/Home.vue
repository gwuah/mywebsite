<template>
  <div class="home">
    <navigation class="navigation"/>

    <h1 class="name">Griffith Asare Awuah</h1>
    <p class="description">I'm a junior software engineer, aspiring product designer and fulltime javscript merchant.</p>
    <p class="current-position">Currently working as a fullstack intern at <a class="aidahbot-text" href="https://www.aidahbot.com">Aidahbot Company</a></p>
    <p class="spread-love">...</p>


    <!-- <img class="code-preview" :src="preview_img"/> -->

    <div class="skills-container normal">
      <skill-tablet class="skill" v-for="(skillset, key) in skills" :skill="skillset.skill" :key="key" :color="skillset.color"/>
    </div>

    <div class="skills-container mobile">
      <skill-tablet class="skill" v-for="(skillset, key) in experienced" :skill="skillset.skill" :key="key" :color="skillset.color"/>
    </div>

    <div class="mini-contact">
      Do I look like your guy? <span class="lets-talk">If yes, then let's talk.</span> <a href="#" class="contact-me" @click.prevent="contactMe">contact me</a>

      <div>
      <a href="https://twitter.com/gwuah_"><i data-feather="twitter"></i></a> |
      <a href="https://www.linkedin.com/in/griffith-awuah-b00a62112/_"><i data-feather="linkedin"></i></a>|
      <a href="https://facebook.com/gwuah_"><i data-feather="facebook"></i></a> |
      <a href="https://github.com/gwuah_"><i data-feather="github"></i></a> |
      </div>

    </div>

  </div>
</template>

<style scoped>
  .navigation {
    margin-bottom: 130px;
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

  .current-position {
    padding: 0 20px;
  }

  .current-position .aidahbot-text {
    text-decoration: none;
  }

  .skills-container {
    /* margin-top: -30px; */
    padding: 10px;
    width: 50%;
    margin: 0 auto;
    border: 1px solid #f1f1f1;
    display: flex;
    flex-flow: row wrap;
    justify-content: space-around
  }

  .mobile {
    display: none
  }

  /* .skill {
    margin: 0 10px 10px 0;
  } */

  .mini-contact {
    /* width: 60%; */
    margin: 0 auto;
    margin-top: 25px !important;
    /* border: 1px solid red; */
    padding: 10px;
    position: relative;
    top: 78px;
    margin-bottom: 30px;
  }

  .contact-me {
    background-color: #fc3;
    color: black;
    padding:4px;
    border-radius: 6px;
    border: 1px solid #f1f1f1;
    margin-left: 4px;
  }

  .mini-contact div {
    margin-top: 10px;
  }

  .mini-contact svg { 
    height: 16px;
    position: relative;
    top: 2px;
    color: black;
  }

  @media (max-width: 1100px) {
    .skills-container {
      width: 90%;
      margin-bottom: 4px;
      /* border: 1px solid red; */
    }
  }

  @media (max-width: 500px) {
    .navigation {
      margin-bottom: 90px;
    }

    h1.name {
      margin-bottom: 50px;
    }

    .skills-container {
      width: 90%;
      margin-bottom: 4px;
      /* border: 1px solid red; */
    }

    .normal {
      display: none;
    }

    .mobile {
      display: flex;
      margin: none;
    }

    .lets-talk {
      display: none;
    }

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
      experienced: [
        {skill:"reactjs", color: " #f1f1f1"},
        {skill:"vuejs", color: ""},
        {skill:"es5/es6", color: null},
        {skill:"python", color: null},
        {skill:"node", color: null}
      ],
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
        {skill:"git", color: null}
      ]
    }
  },
  mounted() {
    // feather ? feather.replace() : alert("there's no feather")
    // eslint-disable-next-line
    feather.replace()
  },
  methods: {
    contactMe() {
      this.$router.push("contact")
    }
  }
}
</script>
