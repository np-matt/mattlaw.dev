<template>
  <v-row
    wrap
    fill-height
    justify="center"
    align="center"
    class="flex-row-reverse"
  >
    <v-col md="5" cols="12" class="text-center">
      <h1>Matt Law [.dev]</h1>
      <v-btn fab icon href="https://github.com/np-matt" target="_blank">
        <i class="fab fa-github"></i>
      </v-btn>
      <v-btn
        fab
        icon
        href="https://www.linkedin.com/in/matthew-law-40659062/"
        target="_blank"
      >
        <i class="fab fa-linkedin"></i>
      </v-btn>
      <v-btn
        fab
        icon
        href="https://twitter.com/Northern_Pariah"
        target="_blank"
      >
        <i class="fab fa-twitter"></i>
      </v-btn>
    </v-col>
    <v-col md="5" cols="12">
      <v-row align="center" class="text-center" justify="center">
        <v-col>
          <v-avatar size="256">
            <img
              src="https://www.gravatar.com/avatar/d1a10bb5688a532548bd960458e093a5.jpg?s=256"
              alt="Me (MattLaw.Dev) and my gorgeous Fiancee Pen!"
            />
          </v-avatar>
        </v-col>
        <v-col>
          <ul class="title">
            <li>Often Programmer</li>
            <li>Occasional DIY-er</li>
            <li>Infrequent Cricketer</li>
          </ul>
        </v-col>
      </v-row>
    </v-col>
  </v-row>
</template>

<style scoped>
.row {
  min-height: 100vh;
}

h1 {
  text-align: center;
  font-weight: 100;
}

ul {
  list-style-type: none;
  padding: 0 !important;
}

li {
  padding: 10px;
}

li {
  margin: 10px 0;
  background: rgba(66, 66, 66, 0.7) !important;
}

i {
  font-size: 2.5em;
}
</style>
