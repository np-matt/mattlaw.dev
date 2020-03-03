<template>
  <v-layout>
    <v-flex shrink>
      <v-btn icon fab>
        <i class="fab fa-facebook" @click.prevent="facebook"></i>
      </v-btn>
      <v-btn icon fab>
        <i class="fab fa-twitter" @click.prevent="twitter"></i>
      </v-btn>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  mounted() {
    const interval = setInterval(() => {
      if (FB) {
        FB.init({
          appId: '339966533613489',
          autoLogAppEvents: true,
          xfbml: true,
          version: 'v4.0',
        });

        clearInterval(interval);
      }
    }, 500);
  },
  methods: {
    facebook() {
      FB.ui(
        {
          method: 'share',
          href: window.location.href,
        },
        function(response) {}
      );
    },
    twitter() {
      window.open(
        'http://twitter.com/share?url=' +
          encodeURIComponent(window.location.href),
        '',
        'left=0,top=0,width=550,height=450,personalbar=0,toolbar=0,scrollbars=0,resizable=0'
      );
    },
  },
};
</script>

<style scoped>
.v-btn >>> i {
  font-size: 40px;
}

.flex {
  margin: auto;
}
</style>
