<template>
  <v-layout column justify-center align-center>
    <ResumeIntroduction />
    <ResumeExperience />
  </v-layout>
</template>

<script>
import ResumeIntroduction from '../components/resume/ResumeIntroduction.vue'
import ResumeExperience from '../components/resume/ResumeExperience.vue'
export default {
  components: {
    ResumeIntroduction,
    ResumeExperience
  }
}
</script>
