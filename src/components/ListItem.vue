<template>
  <v-list-item>
    <v-list-item-icon v-if="icon" class="text-center mr-2">
      <v-icon>{{ icon }}</v-icon>
    </v-list-item-icon>
    <v-list-item-content>
      <v-list-item-title v-if="title" class="text-wrap">
        {{ title }}
      </v-list-item-title>
      <v-list-item-subtitle class="text-wrap">
        <slot>
          {{ subtitle }}
        </slot>
      </v-list-item-subtitle>
    </v-list-item-content>
  </v-list-item>
</template>

<script>
export default {
  props: {
    icon: { type: String },
    title: { type: String },
    subtitle: { type: String },
  },
};
</script>
