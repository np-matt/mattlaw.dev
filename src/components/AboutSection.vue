<template>
  <v-row>
    <v-col cols="12" class="headline pt-2 pb-2">
      <span class="pr-2 pl-2">
        <v-btn fab depressed class="primary">
          <v-icon>{{ icon }}</v-icon>
        </v-btn>
        {{ title }}
      </span>
    </v-col>
    <v-col class="body-1 pt-0 pb-0">
      <slot />
    </v-col>
  </v-row>
</template>

<script>
export default {
  props: ['icon', 'title'],
};
</script>

<style scoped>
.headline {
  position: relative;
}

span {
  background-color: white;
}

.headline:after {
  position: absolute;
  width: 100%;
  left: 0;
  bottom: 50%;
  z-index: -1;
  content: '';
  border-bottom: 1px dashed black;
}

.v-icon {
  font-size: 25px;
}
</style>
