<template>
  <v-card class="projectCard">
    <v-card-title class="headline">{{project.title}}</v-card-title>
    <v-card-subtitle>{{project.subtitle}}</v-card-subtitle>
    <v-card-text>
      <div v-for="line in project.paragraphs" :key="line[0]">{{line}}</div>
    </v-card-text>
    <v-card-actions>
      <v-spacer />
      <v-btn
        v-for="(url, name) in project.links"
        color="primary"
        link
        :href="url"
        :key="url"
      >{{name}}</v-btn>
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
}
</style>
