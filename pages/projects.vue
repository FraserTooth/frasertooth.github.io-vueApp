<template>
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <ProjectsIntroducton />
      <v-card>
        <ProjectAlwyn />
      </v-card>
      <v-card>
        <ProjectGoExamine />
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
import ProjectsIntroducton from '../components/projects/ProjectsIntroduction'
import ProjectAlwyn from '../components/projects/ProjectAlwyn'
import ProjectGoExamine from '../components/projects/ProjectGoExamine'
export default {
  components: { ProjectsIntroducton, ProjectAlwyn, ProjectGoExamine }
}
</script>
