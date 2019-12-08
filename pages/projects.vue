<template>
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <ProjectsIntroducton />
      <ProjectCard v-for="project in projects" :key="project.title" :project="project" />
    </v-flex>
  </v-layout>
</template>

<script>
import ProjectsIntroducton from '../components/projects/ProjectsIntroduction'
import ProjectCard from '../components/projects/ProjectCard'

//  JSON Files for Projects
import projects from '../assets/data/projects/projects.js'
export default {
  components: {
    ProjectsIntroducton,
    ProjectCard
  },
  data() {
    return {
      projects
    }
  }
}
</script>
