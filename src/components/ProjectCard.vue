<template>
  <div class="project-card">
    <div class="project__img">
      <img alt="project-img" :src='project.img'/>
    </div>
    <div class="project__about">
      <div class="project__name">{{project.name}}</div>
      <div class="project__sample">{{project.abstract}}</div>
      <div class="project___stack">{{stacky}}</div>
    </div>
  </div>
</template>

<style scoped>
  .project__img, .project__about {
    border: 1px solid red;
    width: 100%;
  }
  .project__name {
    font-weight: bold;
    text-transform: capitalize;
    margin: 10px;
  }
  .project__sample {
    font-size: 15px;
    margin: 10px;
  }
  .project-card {
    width: 30%;
    border: 1px solid green;
    margin-bottom: 10px;
    padding: 50px;
    box-sizing: border-box;
    font-family: 'Fira Sans Condensed'
  }
</style>

<script>

export default {
  name: "ProjectCard",
  props: {
    project: Object
  },
  data() {
    return {}
  },
  computed :{
    stacky() { return this.project.stack.join(',') }
  }
}
</script>

