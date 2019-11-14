<template>
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <v-layout>
        <ResumeIntroduction />
        <ResumeExperience />
      </v-layout>
    </v-flex>
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
