<template>
  <div class="project-card">
    fdhdf
  </div>
</template>

<style scoped>
  .project-card {
    width: 33%;
    border: 1px solid red;
  }
</style>

<script>

// props: {
//     img: String,
//     name: String,
//     website: String,
//     technologies: Array
// }

export default {
  name: "ProjectCard",
  props: {
    logo: String,
    name: String,
    website: String,
    technologies: Array
  },
  data() {
    return {}
  }
}
</script>

