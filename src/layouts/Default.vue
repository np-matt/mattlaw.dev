<template>
  <v-content>
    <slot />
  </v-content>
</template>

<style lang="scss">
.fade-enter-active {
  transition: opacity 0.2s;
}

.fade-enter {
  opacity: 0;
}
</style>
