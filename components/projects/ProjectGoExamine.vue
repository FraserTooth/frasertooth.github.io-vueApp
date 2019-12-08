<template>
  <v-list-group>
    <template v-slot:activator>
      <v-list-item-title>Go Examine - Fake News Training App</v-list-item-title>
    </template>

    <v-list-item>
      <v-list-item-content>
        <p>App to scrape website and identify ‘fake news’ language usage.</p>
        <p>Browser Extension which sends the url to API, receives a list of locations and highlights ‘problem words’ with hover-over tooltip.</p>
        <p>API Built in Go deployed to Google Cloud Functions.</p>
        <p>
          Project Page:
          <a href="https://github.com/FraserTooth/alwyn">github.com/FraserTooth/alwyn</a>
        </p>
        <p>
          Demo:
          <a href="alwyn.herokuapp.com/">alwyn.herokuapp.com/</a>
        </p>
      </v-list-item-content>
    </v-list-item>

    <v-list-item>
      <v-list-item-content>
        <p>Drag-drop flowchart app that transpiles to Javascript. Built in React & Node.</p>
      </v-list-item-content>
    </v-list-item>
  </v-list-group>
</template>
