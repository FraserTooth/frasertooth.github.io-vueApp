<template>
  <v-list-group active-class="router-link-active" no-action sub-group>
    <template v-slot:activator>
      <v-list-item-content>
        <v-list-item-title>{{jobData.jobTitle}}</v-list-item-title>
      </v-list-item-content>
    </template>

    <v-list-item>
      <v-list-item-content>
        <v-card-subtitle>{{jobData.dates}}</v-card-subtitle>
        <div v-for="line in jobData.lines" :key="line">{{line}}</div>
      </v-list-item-content>
    </v-list-item>
  </v-list-group>
</template>

<script>
export default {
  props: ['jobData']
}
</script>
