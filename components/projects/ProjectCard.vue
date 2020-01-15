<template>
  <v-card class="projectCard">
    <v-card-title class="headline">{{ project.title }}</v-card-title>
    <v-carousel
      v-if="project.pictures"
      height="50vh"
      hide-delimiter-background
      show-arrows-on-hover
      cycle
    >
      <v-carousel-item
        v-for="(pictureUrl,i) in project.pictures"
        :key="i"
        reverse-transition="fade-transition"
        transition="fade-transition"
        :src="pictureUrl"
        contain
      />
    </v-carousel>

    <v-card-subtitle>{{ project.subtitle }}</v-card-subtitle>
    <v-card-text>
      <div v-for="(line, index) in project.paragraphs" :key="index">{{ line }}</div>
    </v-card-text>
    <v-card-actions>
      <v-spacer />
      <v-flex>
        <v-btn v-for="(url, name) in project.links" :key="url" link :href="url">{{ name }}</v-btn>
      </v-flex>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
  props: ['project']
}
</script>

<style>
.projectCard {
  width: 90vw;
  margin-bottom: 10px;
}
</style>
