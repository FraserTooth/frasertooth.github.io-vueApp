<template>
  <v-card class="jobCard">
    <v-card-title class="headline">{{experienceData.company}}</v-card-title>
    <v-card-subtitle>{{experienceData.subtitle}}</v-card-subtitle>
    <Job v-for="jobData in experienceData.jobs" :jobData="jobData" :key="jobData.jobTitle[0]" />
    <v-card-text>
      <div v-for="line in experienceData.paragraphs" :key="line[0]">{{line}}</div>
    </v-card-text>
    <v-card-actions>
      <v-spacer />
      <v-btn
        v-for="(url, name) in experienceData.links"
        color="primary"
        link
        :href="url"
        :key="url"
      >{{name}}</v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
import Job from './Job.vue'
export default {
  components: { Job },
  props: ['experienceData']
}
</script>

<style>
.jobCard {
  width: 90vw;
}
</style>
