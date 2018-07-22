<template>
  <div>
    <navigation/>
    
    <div>contact page</div>
  </div>
</template>

<style scoped>
  .navigation {
    margin-bottom: 150px;
  }


</style>


<script>

import Navigation from '@/components/Navigation';
import SkillTablet from '@/components/SkillTablet';

export default {
  name: 'contactMe',
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
  },
  methods: {
    contactMe() {
      this.$router.push("contact")
    }
  }
}
</script>
