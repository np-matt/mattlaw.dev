<template>
  <v-container>
    <v-row align-content="center" justify="center">
      <v-col cols="10">
        <h2 data-aos="fade-down" class="text-center drop">
          I have experience architecting &amp; developing complex web apps
        </h2>
      </v-col>
      <v-col
        cols="12"
        sm="6"
        md="4"
        class="d-flex"
        v-for="(project, i) of projects"
        :key="project.title"
      >
        <v-card
          outlined
          tile
          data-aos="fade-up"
          :data-aos-delay="100 * (i + 1)"
        >
          <g-image
            :src="require(`!!assets-loader!@images/${project.img}`)"
            :alt="project.title"
            height="252px"
            v-if="project.img"
          />
          <div v-else class="placeholder">
            <div
              class="placeholder__inner d-flex align-center justify-center flex-column"
            >
              <v-icon size="50px">{{ mdiImage }}</v-icon>
              <p class="subtitle-1">Image not available</p>
            </div>
          </div>
          <v-card-title class="text-center">{{ project.title }}</v-card-title>
          <v-card-text>{{ project.abstract }}</v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import { mdiImage } from '@mdi/js';

export default {
  setup() {
    return {
      mdiImage,
      projects: [
        {
          title: 'Distributed Training Systems',
          abstract:
            'Integration of real & simulated equipment all driven via a web-based interface. This included a 2D map display of simulated entities and scenario generation using the Distributed Interactive Simulation (DIS) network protocol & VR Forces.',
        },
        {
          title: 'helpmystreet.org',
          abstract:
            'As part of my role at Distinction I created the Frontend .NET MVC Core application & architecture for integrating with the database-driven microservices.',
          img: 'hms.png',
        },
        {
          title: 'mattlaw.dev',
          abstract:
            "This very site built with VueJS and Gridsome! Over the past few months I've integrated a few different Content Management Systems to get a feel for them, including Kentico Kontent, Prismic & Netlify CMS.",
          img: 'screenshot.png',
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.placeholder {
  position: relative;
  width: 100%;
  background-color: lightgrey;
  padding-top: 9 / 16 * 100%;

  &__inner {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
}
</style>
