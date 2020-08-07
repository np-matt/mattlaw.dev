<template>
  <v-app :class="{ 'bg-green': $route.name === 'home' }">
    <v-app-bar color="primary" dark dense fixed :value="showBar" :app="isApp">
      <v-toolbar-items>
        <v-tooltip bottom>
          <template v-slot:activator="{ on }">
            <v-btn to="/" icon v-on="on" aria-label="Home">
              <v-icon dark>{{ mdiHome }}</v-icon>
            </v-btn>
          </template>
          <span>Home</span>
        </v-tooltip>
        <v-tooltip bottom>
          <template v-slot:activator="{ on }">
            <v-btn to="/about" icon v-on="on" aria-label="About">
              <v-icon>{{ mdiClipboardAccountOutline }}</v-icon>
            </v-btn>
          </template>
          <span>About</span>
        </v-tooltip>
        <v-tooltip bottom>
          <template v-slot:activator="{ on }">
            <v-btn to="/blog" icon v-on="on" aria-label="Blog">
              <v-icon>{{ mdiNewspaper }}</v-icon>
            </v-btn>
          </template>
          <span>Blog</span>
        </v-tooltip>
      </v-toolbar-items>
      <v-spacer />
      <v-toolbar-items>
        <v-tooltip bottom>
          <template v-slot:activator="{ on }">
            <v-btn
              icon
              href="https://github.com/mlawd"
              target="_blank"
              role="button"
              aria-label="GitHub"
              rel="noopener"
              v-on="on"
            >
              <v-icon>{{ mdiGithub }}</v-icon>
            </v-btn>
          </template>
          <span>GitHub</span>
        </v-tooltip>
        <v-tooltip bottom>
          <template v-slot:activator="{ on }">
            <v-btn
              icon
              href="https://twitter.com/mattlawdev"
              target="_blank"
              role="button"
              aria-label="Twitter"
              rel="noopener"
              v-on="on"
            >
              <v-icon>{{ mdiTwitter }}</v-icon>
            </v-btn>
          </template>
          <span>Twitter</span>
        </v-tooltip>
        <v-tooltip bottom>
          <template v-slot:activator="{ on }">
            <v-btn
              icon
              href="https://www.linkedin.com/in/mattlawdev"
              target="_blank"
              role="button"
              aria-label="LinkedIn"
              rel="noopener"
              v-on="on"
            >
              <v-icon>{{ mdiLinkedin }}</v-icon>
            </v-btn>
          </template>
          <span>LinkedIn</span>
        </v-tooltip>
      </v-toolbar-items>
    </v-app-bar>
    <router-view />
    <v-btn fab fixed bottom left v-if="isDev">
      {{ $vuetify.breakpoint.name }}
    </v-btn>
  </v-app>
</template>

<static-query>
query {
  metadata {
    siteName
    siteDescription
  }
}
</static-query>

<script>
import {
  mdiHome,
  mdiTwitter,
  mdiGithub,
  mdiLinkedin,
  mdiClipboardAccountOutline,
  mdiNewspaper,
  mdiCodeJson,
} from '@mdi/js';
import { watch, ref } from '@vue/composition-api';

export default {
  setup(
    _,
    {
      root: { $route },
    }
  ) {
    const showBar = ref($route.name !== 'home');
    const isApp = ref($route.path !== '/about');

    console.log($route);

    watch('$route.path', newVal => {
      isApp.value = newVal !== '/about';
    });

    watch('$route.name', newVal => {
      showBar.value = newVal !== 'home';
    });

    return {
      mdiHome,
      mdiTwitter,
      mdiGithub,
      mdiLinkedin,
      mdiClipboardAccountOutline,
      mdiNewspaper,
      mdiCodeJson,
      showBar,
      isApp,
      isDev: process.env.NODE_ENV !== 'production',
    };
  },
};
</script>
