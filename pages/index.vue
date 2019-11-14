<template>
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <v-card>
        <v-card-title class="headline">Welcome to Fraser's Website</v-card-title>
        <v-card-text>
          <p>Hi, I'm Fraser Tooth 🦷</p>
          <p>I'm a Full Stack Development Bootcamp student living in Tokyo, Japan. 🗾</p>
          <p>I'm originally from Scotland 🏴󠁧󠁢󠁳󠁣󠁴󠁿</p>
          <p>Please have a look around!</p>
          <p>This website was built with Nuxt.js</p>
          <p>Its not yet filled with all the content I'd like to put here.</p>
          <p>I'm quite busy at the Bootcamp so will update when I have spare time!</p>
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn color="primary" nuxt to="/resume">Resume</v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  components: {}
}
</script>
