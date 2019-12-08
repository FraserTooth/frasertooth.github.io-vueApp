<template>
  <v-layout column justify-center align-center>
    <ResumeIntroduction />
    <CompanyCard :experienceData="kiwiData" />
  </v-layout>
</template>

<script>
import ResumeIntroduction from '../components/resume/ResumeIntroduction.vue'
import CompanyCard from '../components/experience/CompanyCard.vue'

//  JSON Files for Jobs
import kiwiData from '../assets/data/experience/kiwipower.json'
export default {
  components: {
    ResumeIntroduction,
    CompanyCard
  },
  data() {
    return {
      kiwiData
    }
  }
}
</script>
