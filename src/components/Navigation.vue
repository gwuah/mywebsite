<template>
  <nav>
    <ul>
      <router-link to="/">home</router-link>|
      <router-link to="/about">about</router-link>|
      <router-link to="/projects">projects</router-link>
    </ul>
  </nav>
</template>

<style scoped>
  nav {
    margin: 70px 0;
  }

  ul {
    -webkit-padding-start: 0px;
  }

  ul a {
    /* text-decoration:; */
    color: black;
    padding: 10px;
  }

  @media (max-width: 500px) {
    nav {margin: 50px 0;}
  }
</style>

<script>
export default {
  name: "Naviagtion"
}
</script>


