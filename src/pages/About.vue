<template>
  <Layout>
    <v-container class="pt-0">
      <v-row>
        <v-col class="pt-0">
          <h1 class="d-none d-print-block mt-n3">
            Matthew Law
          </h1>
          <h1 class="d-print-none">About Me</h1>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="12" class="text-center pa-0">
          <v-chip
            color="primary"
            class="ma-1"
            v-for="{ icon, text } in skills"
            :key="text"
          >
            <v-icon v-text="icon" />&nbsp;{{ text }}
          </v-chip>
        </v-col>
      </v-row>
      <v-row class="flex-row-reverse d-print-block">
        <v-col cols="12" md="5" class="side">
          <v-card>
            <v-card-text class="pa-1 primary">
              <v-subheader class="title">Contact Information</v-subheader>
              <v-list dense subheader class="pt-2">
                <ListItem icon="mdi-email" title="me@mattlaw.dev" />
                <ListItem
                  icon="mdi-web"
                  title="mattlaw.dev"
                  class="d-none d-print-flex"
                />
                <ListItem icon="mdi-github-circle" title="np-matt" />
                <ListItem icon="mdi-linkedin" title="mattlawdev" />
              </v-list>
              <v-subheader class="title">Education</v-subheader>
              <v-list dense subheader class="pt-2">
                <ListItem
                  icon="mdi-school"
                  title="University of Newcastle upon Tyne"
                >
                  1st BSc Computer Science with Industrial Placement (Games
                  Engineering)
                  <ul class="mt-2">
                    <li>Web Technologies</li>
                    <li>Programming for Games</li>
                    <li>Graphics for Games</li>
                    <li>Database Technology</li>
                  </ul>
                </ListItem>
                <ListItem
                  icon="mdi-school-outline"
                  title="Notre Dame High School"
                >
                  3 A-Levels
                  <ul class="mt-2">
                    <li>Maths (A)</li>
                    <li>Physics (B)</li>
                    <li>ICT (B)</li>
                  </ul>
                </ListItem>
              </v-list>
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" md="7">
          <p>
            I am a Web Developer currently working for Solutions for Retail
            Brands on a range of web services.
          </p>
          <p>
            I have a keen interest in various technologies, and whilst most of
            my time at work is spent working in NodeJS and AngularJS, I have
            various personal projects that allow me to keep up to date with
            VueJS, .NET, React &amp; GraphQL. For instance, my website is
            written in VueJS &amp; Gridsome, whilst I have ongoing projects for
            a .NET Core GraphQL Movie API &amp; React front-end. All of which
            can be viewed on my GitHub account.
          </p>
          <v-subheader class="title">
            May '18 - present: Web Developer
          </v-subheader>
          <v-subheader class="font-italic">
            Solutions for Retail Brands (S4RB)
          </v-subheader>
          <p>
            My current role is that of Web Developer for a company providing
            online portals for own-brand supplier engagement.
          </p>
          <p>
            When first starting in the job, my main role was the maintenance and
            development of new features for a monolithic legacy application
            written in NodeJS &amp; AngularJS. This provided a particular
            challenge due to it being a large single-tenant application with a
            multi-client code-base.
          </p>
          <p>
            I was part of the 3 person team responsible for the recent migration
            of these legacy systems from AWS to Azure. This involved the
            dockerisation of applications and creation of new build processes
            within the CircleCI environment, to replace the Heroku build
            pipelines previously in place.
          </p>
          <ul>
            <li>
              Maintenance of large AngularJS &amp; Express NodeJS application
            </li>
            <li>Migrated existing legacy systems from AWS to Azure</li>
            <li>
              Management of CircleCI build pipelines to build and publish
              dockerised applications
            </li>
            <li>
              Design &amp; Development of Azure Function &amp; Service Bus Queue
              based microservices for data processing and RESTful endpoints
            </li>
            <li>
              Successfully promoted the use of VueJS &amp; static hosting for
              all new front-end applications
            </li>
            <li>
              Codification of Logic Apps used to process data from external
              sources in to application databases
            </li>
            <li>
              Unit testing of application code using either Mocha &amp; Chai or
              Jest
            </li>
            <li>
              End to end testing of applications via Cypress
            </li>
          </ul>
          <br />
          <br />
          <v-subheader class="title">
            Aug '17 - Apr '18: Senior Engineer &amp; Technical Lead <br />
            Aug '15 - Aug '17: Graduate Engineer <br />
            Sep '13 - Sep '14: Undergraduate Engineer <br />
          </v-subheader>
          <v-subheader class="font-italic">
            MBDA - Weapon Systems Simulations &amp; Experimentation
          </v-subheader>
          <p>
            From September 2013 to September 2014 I undertook a year out from
            University at MBDA in the Weapon Systems Simulation &amp;
            Experimentation department, creating distributed simulations of
            production equipment for testing and training purposes.
          </p>
          <p>
            During this time I developed the departmental intranet and
            maintained C# libraries used for sub-system simulations. I was also
            heavily involved in the creation and delivery of presentations to
            key customers (both potential and existing) and developed a C++
            NodeJS addon that wrapped an existing C++ library for interacting
            with the DIS network protocol.
          </p>
          <p>
            At the end of my Undergraduate year I was asked to commit to
            returning as a Graduate Engineer pending the successful completion
            of my final year of University.
          </p>
          <p>
            Starting on the Graduate Scheme in August 2015, I worked in multiple
            roles including Developer and Delivery Lead, finishing the Graduate
            scheme as a Senior Engineer and the Technical Lead for 2 separate
            simulation systems. I also took courses on Agile Fundamentals,
            Presentation Skills, Negotiation and Project Management.
          </p>
          <ul>
            <li>
              Led the development of key software components for an in-house
              framework built upon C# and .NET Framework version 4.0
            </li>
            <li>
              Drove the adoption of web technologies including NodeJS coupled
              with C# &amp; C++ applications to deliver an Instructor &amp;
              Operator Station that can run within a web-browser
            </li>
            <li>
              Design authority responsible for creating system and software
              architectures, sequence diagrams &amp; data exchange
              specifications/APIs
            </li>
            <li>
              C++ development of VBS3 plugins &amp; libraries
            </li>
            <li>
              Co-ordinated a pan-european team of software developers
            </li>
            <li>
              Provided daily reports to Cheif Engineers in the run-up to key
              integration events
            </li>
          </ul>
          <v-subheader class="title mb-2">Personal Interests</v-subheader>
          <p>
            Outside of work I enjoy working on my own projects, usually as a way
            to keep up to date on technologies that I do not necessarily have
            the opportunity to work with at my job.
          </p>
          <p>
            For instance, the previously mentioned GraphQL Movie API that is a
            wrapper around The Movie Database REST API, and accompanying React
            frontend. Both projects I undertook so as to provide myself an
            opportunity to work with .NET Core, GraphQL &amp; React; all of
            which are technologies not used in my current role but which I have
            a keen interest in.
          </p>
          <p>
            I have also developed my own blog using Vue, Vuetify &amp; Gridsome,
            as a way to familiarise myself with static site generators, Netlify
            and JAMStack applications.
          </p>
          <p>
            Prior to that I developed my own CMS system using ApolloServer that
            I deployed to DigitalOcean using Docker images automatically built
            using CircleCI and deployed via Kubernetes.
          </p>
          <p>
            I enjoy being involved in sports teams. I have recently joined a
            Cricket club as well as having played Football and Basketball,
            including representing my city at National League level for the
            Junior Sharks Basketball Team. I spent 2 years as captain of the
            Junior Sharks B Team, 2 years as Captain of the Newcastle University
            Knights &amp; 2 years as President of the Newcastle University
            Knights.
          </p>
          <p class="mb-0">
            I am also a Level 2 Basketball coach and have previously coached
            Basketball to a high level, reaching the National League Playoff
            Finals 3 years running, winning in the 3rd year.
          </p>
        </v-col>
      </v-row>
    </v-container>
  </Layout>
</template>

<script>
import ListItem from '../components/ListItem.vue';

export default {
  metaInfo: { title: 'About me' },
  components: { ListItem },
  data() {
    return {
      skills: [
        { icon: 'mdi-language-csharp', text: 'C#' },
        { icon: 'mdi-dot-net', text: '.NET' },
        { icon: 'mdi-language-cpp', text: 'C++' },
        { icon: 'mdi-language-javascript', text: 'JavaScript' },
        { icon: 'mdi-language-typescript', text: 'TypeScript' },
        { icon: 'mdi-language-css3', text: 'CSS' },
        { icon: 'mdi-language-html5', text: 'HTML' },
        { icon: 'mdi-nodejs', text: 'NodeJS' },
        { icon: 'mdi-vuejs', text: 'VueJS' },
        { icon: 'mdi-vuetify', text: 'Vuetify' },
        { icon: 'mdi-react', text: 'React' },
        { icon: 'mdi-angular', text: 'Angular' },
        { icon: 'mdi-graphql', text: 'GraphQL' },
        { icon: 'mdi-kubernetes', text: 'Kubernetes' },
        { icon: 'mdi-docker', text: 'Docker' },
        { icon: 'mdi-database', text: 'MongoDB' },
        { icon: 'mdi-database', text: 'SQL' },
        { icon: 'mdi-database', text: 'Snowflake' },
        { icon: 'mdi-azure', text: 'Azure' },
        { icon: 'mdi-aws', text: 'AWS' },
        { icon: 'mdi-cloud-outline', text: 'DigitalOcean' },
      ],
    };
  },
};
</script>

<style scoped>
.title {
  color: black !important;
}

h2,
h3 {
  text-decoration: underline;
  text-decoration-color: #5f9ea0;
}

.v-subheader {
  height: inherit;
  min-height: 48px;
}

@media print {
  .side {
    width: 40%;
    float: right;
  }

  .v-application .title {
    font-size: 1.7em !important;
  }
}
</style>
