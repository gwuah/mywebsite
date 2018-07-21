<template>
  <div>
    <navigation/>

    <div class="projects">
    This is my products page
    </div>
  </div>
</template>

<style scoped>

</style>


<script>

import Navigation from '@/components/Navigation'


export default {
  name: 'projects',
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
