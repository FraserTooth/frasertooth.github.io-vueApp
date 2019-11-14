<template>
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <v-layout>
        <v-card>
          <v-flex class="text-center">
            <v-card-title class="headline">Fraser Tooth</v-card-title>
            <ResumeIntroduction />
          </v-flex>
        </v-card>
      </v-layout>
    </v-flex>
  </v-layout>
</template>

<script>
import ResumeIntroduction from '../components/resume/ResumeIntroduction.vue'
export default {
  components: {
    ResumeIntroduction
  }
}
</script>
