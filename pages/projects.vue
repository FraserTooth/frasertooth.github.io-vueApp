<template>
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <ProjectsIntroducton />
      <ProjectCard :projectData="alwynData" />
      <ProjectCard :projectData="goExamineData" />
    </v-flex>
  </v-layout>
</template>

<script>
import ProjectsIntroducton from '../components/projects/ProjectsIntroduction'
import ProjectCard from '../components/projects/ProjectCard'

//  JSON Files for Projects
import alwynData from '../assets/data/projects/alwyn.json'
import goExamineData from '../assets/data/projects/goexamine.json'
export default {
  components: {
    ProjectsIntroducton,
    ProjectCard
  },
  data() {
    return {
      alwynData,
      goExamineData
    }
  }
}
</script>
