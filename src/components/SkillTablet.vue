<template>

  <div :style="{backgroundColor: color || '#fc3' }">{{skill}}</div>
  
</template>

<style scoped>
  div {
    /* background-color: #fc3; */
    padding: 5px;
    border-radius: 4px;
  }
</style>

<script>
export default {
  name: "skillTablet",
  props: {
    skill: String,
    color: String
  },
  data() {
    return {}
  }
}
</script>

