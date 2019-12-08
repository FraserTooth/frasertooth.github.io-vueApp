<template>
  <v-card>
    <v-card-title class="headline">{{projectData.title}}</v-card-title>
    <v-card-subtitle>{{projectData.subtitle}}</v-card-subtitle>
    <v-card-text>
      <div v-for="line in projectData.paragraphs" :key="line[0]">{{line}}</div>
    </v-card-text>
    <v-card-actions>
      <v-spacer />
      <v-btn
        v-for="(url, name) in projectData.links"
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
  props: ['projectData']
}
</script>
