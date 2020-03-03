<template>
  <div>
    <ListItem :title="title" />

    <v-list-item>
      <v-row class="ma-0">
        <v-col
          v-for="({ icon, text }, i) of skills"
          :key="text"
          cols="6"
          xl="4"
          class="pa-0 pr-1"
        >
          <v-list-item class="pl-0">
            <v-list-item-icon class="mr-2">
              <v-icon v-text="icon"></v-icon>
            </v-list-item-icon>
            <v-list-item-content>{{ text }}</v-list-item-content>
          </v-list-item>
        </v-col>
      </v-row>
    </v-list-item>
  </div>
</template>

<script>
import ListItem from './ListItem.vue';

export default {
  components: { ListItem },
  props: {
    title: { type: String, required: true },
    skills: { type: Array, required: true },
  },
};
</script>
