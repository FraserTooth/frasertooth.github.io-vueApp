<template>
  <v-layout column justify-center align-center>
    <ResumeIntroduction />
    <ResumeProjects />
    <ResumeExperience />
  </v-layout>
</template>

<script>
import ResumeIntroduction from '../components/resume/ResumeIntroduction.vue'
import ResumeExperience from '../components/resume/ResumeExperience.vue'
import ResumeProjects from '../components/resume/ResumeProjects.vue'
export default {
  components: {
    ResumeIntroduction,
    ResumeExperience,
    ResumeProjects
  }
}
</script>
