<template>
  <div>
    <navigation class="navigation"/>

    <h3>A couple of things I have built .</h3>

    <div class="projects">
      <project-card class="project-card" v-for="(project, key) in projects" :key="key" :project='project'/>
    </div>
  </div>
</template>

<style scoped> 
  /* * {
    border: 1px solid red;
  } */

  h3 { 
    font-family: 'Fira Sans Condensed'
  }

  .navigation {
    margin-bottom: 50px;
  }

  .projects {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    flex-flow: row wrap;
  }

  .project-card {
  }

</style>


<script>

import Navigation from '@/components/Navigation';
import ProjectCard from '@/components/ProjectCard';


export default {
  name: 'projects',
  components: {
    Navigation,
    ProjectCard
  },
  data() {
    return {
      projects: [{
        name: 'axel',
        stack: ['js', 'typescript'],
        abstract: 'A tiny js lib that allows you to create unique containers per namespace in local-storage.',
        github: 'https://github.com/gwuah/axel',
        liveUrl: '',
      },
      {
        name: 'dropout',
        stack: ['node', 'mongo', 'express', 'html', 'css', 'jquery'],
        abstract: 'An application that allows you to pair program with anybody in realtime',
        github: 'https://github.com/gwuah/dropout',
        liveUrl: 'https://dropout-kilm.herokuapp.com/'
      },
      {
        name: 'sherperd',
        stack: ['node'],
        abstract: 'A tiny service that grows your twitter account for you. [WIP]',
        github: 'https://github.com/gwuah/sherperd',
        liveUrl: ''
      },
      {
        name: 'adsumo',
        stack: ['node', 'vue', 'express', 'mongodb', 'html+css'],
        abstract: 'An online restaurant management system, with 2 dashboards built with vuejs for admins and clients',
        github: '',
        liveUrl: 'http://adsumo.herokuapp.com/'
      },
      {
        name: 'twit-traction',
        stack: ['node'],
        abstract: 'A node script that allows you to gain more views per tweet. [ good for advertisements ]',
        github: 'https://github.com/gwuah/twit-traction',
        liveUrl: ''
      },
      {
        name: 'xenar',
        stack: ['node'],
        abstract: 'A chrome extension that prevents websites from minning crypto with your resources. Runs custom malware scanner every second.',
        github: 'https://github.com/gwuah/xenar',
        liveUrl: ''
      },
      {
        name: 'cryptomaniac',
        stack: ['html', 'css', 'js'],
        abstract: 'A chrome extension to keep track of the top 6 crypto-currencies in real time.',
        github: 'https://github.com/gwuah/crypto-maniac',
        liveUrl: ''
      },
      {
        name: 'twitter-save',
        stack: ['html', 'css', 'js'],
        abstract: 'A chrome extension that enables you to save tweets for later reference!',
        github: 'https://github.com/gwuah/twitter-save',
        liveUrl: ''
      },
      {
        name: 'kerious',
        stack: ['node', 'express', 'mongodb','vuejs'],
        abstract: 'A minimal version of curious cat.',
        github: 'https://github.com/gwuah/kerious',
        liveUrl: ''
      },
      {
        name: 'heatmap',
        stack: ['javascript'],
        abstract: 'A tiny lib that generates user activity heat-maps on your website.',
        github: ' https://github.com/gwuah/heatmap',
        liveUrl: ''
      },
      {
        name: 'ogma',
        stack: ['python'],
        abstract: 'A tiny python wrapper around the languagelayer api.',
        github: 'https://github.com/gwuah/ogma',
        liveUrl: '',
      },
      {
        name: 'udemy-link-extractor',
        stack: ['python'],
        abstract: 'A python program that extracts lecture video links of a Udemy course',
        github: 'https://github.com/gwuah/udemy-course-link-extractor',
        liveUrl: '',
      },
      {
        name: 'axel',
        stack: ['js', 'typescript'],
        abstract: 'A tiny js lib that allows you to create unique containers per namespace in local-storage.',
        github: 'https://github.com/gwuah/axel',
        liveUrl: '',
      }],
      preview_img: "./previewg.png"
    }
  }
}

// https://github.com/gwuah/heatmap
</script>
