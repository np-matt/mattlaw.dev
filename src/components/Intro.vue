<template>
  <v-row justify="center" class="fill-height">
    <v-col md="8">
      <v-row cols="12" justify="center" align="center">
        <v-col
          class="headline-text text-center"
          :class="{ 'headline-text-sm': $vuetify.breakpoint.smAndDown }"
        >
          <p>ABOUT ME</p>
        </v-col>
      </v-row>
      <v-row cols="12" justify="center" align="center">
        <v-col cols="12" class="text-center title">
          <p>
            Welcome to MattLaw.dev! I am a software developer from Sheffield,
            educated at Newcastle University and based in Nottingham.
          </p>
          <p>
            I have experience in Software Development ranging from real-time
            software applications for simulation &amp; training applications to
            enterprise-application web development.
          </p>
          <p>
            Here you will find my thoughts on all things software development,
            NodeJS, .NET, VueJS, WebGL &amp; pretty much anything that takes my
            fancy.
          </p>
          <p>
            <g-link to="/about2" class="text-decoration-none">
              Want to know more?
            </g-link>
          </p>
        </v-col>
      </v-row>
    </v-col>
  </v-row>
</template>

<style scoped>
a {
  text-decoration: none;
}

.fill-height {
  min-height: 100vh;
}

img {
  position: absolute;
  width: 100%;
  mix-blend-mode: darken;
}

p {
  line-height: 1;
}

.headline-text {
  position: relative;
  z-index: 99;
  font-family: 'PT Sans Narrow', sans-serif;
  font-weight: 700;
  font-size: 9em;
  position: relative;
  overflow-y: hidden;
  background: url('/img/nottingham.webp') center;
  background-size: cover;
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
  margin: 30px 0;
}

.headline-text-sm {
  font-size: 5.5em;
}

.intro p {
  font-size: 2.5vw;
}
</style>
