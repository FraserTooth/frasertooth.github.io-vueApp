<template>
  <v-card class="jobCard">
    <v-card-title class="headline">{{ experienceData.company }}</v-card-title>
    <v-carousel
      v-if="experienceData.pictures"
      height="50vh"
      hide-delimiter-background
      show-arrows-on-hover
      cycle
    >
      <v-carousel-item
        v-for="(pictureUrl,i) in experienceData.pictures"
        :key="i"
        reverse-transition="fade-transition"
        transition="fade-transition"
        :src="pictureUrl"
        contain
      />
    </v-carousel>
    <v-card-subtitle>{{ experienceData.subtitle }}</v-card-subtitle>
    <Job v-for="jobData in experienceData.jobs" :key="jobData.jobTitle" :job-data="jobData" />
    <v-card-text>
      <div v-for="(line, index) in experienceData.paragraphs" :key="index">{{ line }}</div>
      <v-spacer />
      <v-btn v-for="(url, name) in experienceData.links" :key="url" link :href="url">{{ name }}</v-btn>
    </v-card-text>
    <v-card-actions />
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
  margin-top: 10px;
}
</style>
