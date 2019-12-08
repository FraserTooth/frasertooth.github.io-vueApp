<template>
  <v-layout column justify-center align-center>
    <ResumeIntroduction />
    <CompanyCard v-for="company in companies" :experienceData="company" :key="company.company" />
  </v-layout>
</template>

<script>
import ResumeIntroduction from '../components/resume/ResumeIntroduction.vue'
import CompanyCard from '../components/experience/CompanyCard.vue'

//  JSON Files for Jobs
import companies from '../assets/data/experience/experience.js'
export default {
  components: {
    ResumeIntroduction,
    CompanyCard
  },
  data() {
    return {
      companies
    }
  }
}
</script>
