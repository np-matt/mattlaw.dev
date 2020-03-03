<template>
  <aside>
    <p class="display-1 font-weight-bold text-center">
      Matthew Law
    </p>
    <p class="headline font-weight-bold text-center">
      Developer
    </p>
    <v-list dense subheader class="primary pt-2" dark>
      <v-subheader class="subtitle-1">Details</v-subheader>
      <ListItem icon="mdi-email" title="me@mattlaw.dev" />
      <ListItem icon="mdi-cellphone-basic" title="07968 897 388" />
      <ListItem
        icon="mdi-web"
        title="mattlaw.dev"
        class="d-none d-print-flex"
      />
      <ListItem icon="mdi-github-circle" title="np-matt" />
      <ListItem icon="mdi-linkedin" title="mattlawdev" />
      <v-subheader class="subtitle-1">Education</v-subheader>
      <ListItem title="Newcastle University">
        1st Class (Hons) BSc Computer Science
      </ListItem>
      <ListItem title="Notre Dame High School">
        3 A-Levels: Maths, Physics &amp; ICT
      </ListItem>
    </v-list>
    <v-subheader class="subtitle-1 pl-2" dark>Skills</v-subheader>
    <p class="text-center">
      <v-icon
        class="ma-1 white--text "
        v-for="{ icon, text } in skills"
        :key="icon"
        v-text="icon"
        style="font-size: 35px"
      />
    </p>
    <v-list dense subheader class="primary" dark>
      <v-subheader class="subtitle-1" dark>Hobbies</v-subheader>
      <ListItem icon="mdi-cricket" title="Cricket" />
      <ListItem icon="mdi-soccer" title="Football" />
      <ListItem icon="mdi-basketball" title="Basketball" />
      <ListItem icon="mdi-tools" title="DIY Projects" />
      <ListItem icon="mdi-code-braces" title="Programming" />
      <ListItem icon="mdi-controller-classic" title="Computer Games" />
    </v-list>
  </aside>
</template>

<script>
import ListItem from '../components/ListItem.vue';

export default {
  components: { ListItem },
  data() {
    return {
      skills: [
        { icon: 'mdi-language-csharp' },
        { icon: 'mdi-dot-net' },
        { icon: 'mdi-language-cpp' },
        { icon: 'mdi-language-javascript' },
        { icon: 'mdi-language-typescript' },
        { icon: 'mdi-language-css3' },
        { icon: 'mdi-language-html5' },
        { icon: 'mdi-nodejs' },
        { icon: 'mdi-vuejs' },
        { icon: 'mdi-react' },
        { icon: 'mdi-angular' },
        { icon: 'mdi-kubernetes' },
        { icon: 'mdi-docker' },
        { icon: 'mdi-azure' },
        { icon: 'mdi-aws' },
        { icon: 'mdi-git' },
      ],
    };
  },
};
</script>

<style>
.v-chip .v-icon {
  font-size: 25px;
}
</style>
