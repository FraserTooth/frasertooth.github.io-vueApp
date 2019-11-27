<template>
  <v-card width="60vw">
    <v-flex class="text-center">
      <v-card-title class="headline">Projects</v-card-title>
      <v-card-subtitle>Things I've Done</v-card-subtitle>
      <ProjectAlwyn />
    </v-flex>
  </v-card>
</template>

<script>
import ProjectAlwyn from './projects/ProjectAlwyn'
export default {
  components: {
    ProjectAlwyn
  }
}
</script>
