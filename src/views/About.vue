<template>
  <div class="about">
    <navigation/>
    
    <h1>This is an about page</h1>

    <project-card/>
  </div>
</template>

<style scoped>

</style>

<script>
import Navigation from '@/components/Navigation'
import ProjectCard from '@/components/ProjectCard'

export default {
  name: "About",
  components: {
    Navigation,
    ProjectCard
  }
}
</script>

