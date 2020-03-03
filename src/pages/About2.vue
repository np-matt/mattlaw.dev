<template>
  <Layout>
    <v-container class="pt-0">
      <v-row>
        <v-col
          cols="3"
          class="primary d-none d-print-block"
          style="height: 200vh; color: white"
        >
          <AboutSideBar />
        </v-col>
        <v-col cols="9" class="pl-8 pr-8">
          <AboutSection title="About me" icon="mdi-account-question">
            <p>
              I am an enthusiastic and hard-working Software Engineer currently
              working as a Web Developer on enterprise applications, with a
              range of experiences including distributed simulations for
              integration and training purposes.
            </p>
            <p>
              Always looking to improve myself and my skills, I have a genuine
              enjoyment of learning new technologies. This is demonstrated by my
              personal projects that utilise React, Agular &amp; GraphQL amongst
              other frameworks and technologies.
            </p>
            <p>
              I am a good team member, having participated in team sports since
              a young age. I have shown throughout my career, both
              professionally and within sports teams, that I also have the
              ability to take on leadership roles when the opportunity arises.
            </p>
          </AboutSection>
          <AboutSection title="Experience" icon="mdi-worker">
            <p class="d-flex justify-space-between align-center title mb-0">
              <span>Web Developer</span>
              <span class="body-1">May 18 - Present</span>
            </p>
            <v-subheader class="pl-0 mb-2 mt-2 font-italic">
              Solutions for Retail Brands (S4RB)
            </v-subheader>
            <p>
              My role initially was the maintenance and development of new
              features for a monolithic legacy application written in NodeJS
              &amp; AngularJS. This provided a particular challenge due to it
              being a large single-tenant application with a multi-client
              code-base.
            </p>
            <p>
              I am currently part of the 3-person team responsible for the
              re-platforming of these legacy systems from AWS to Azure. This has
              involved the dockerisation of applications and creation of new
              build processes within the CircleCI environment, to replace the
              Heroku build pipelines previously in place.
            </p>
            <ul>
              <li>
                Delivery of software components within an agile environment
                including kanban and pair programming
              </li>
              <li>
                Maintenance of an AngularJS &amp; Express NodeJS application
              </li>
              <li>
                Migrated existing legacy systems from AWS to Azure due to
                customer requirements
              </li>
              <li>
                Dockerisation of existing applications to deploy to Azure App
                Services
              </li>
              <li>
                Simplification of existing applications to serverless Azure
                Functions &amp; Logic Apps where appropriate
              </li>
              <li>
                Development of CircleCI workflows to build, publish &amp; deploy
                various applications (docker containers, static web sites &amp;
                functions etc.)
              </li>
              <li>
                Design &amp; Development of Azure Function &amp; Service Bus
                Queue based microservices for data processing and RESTful APIs
              </li>
              <li>
                Successfully promoted the use of VueJS &amp; static hosting for
                new front-end applications
              </li>
              <li>
                Codification of Logic Apps used to process data from external
                sources in to application databases
              </li>
              <li>
                Unit testing of application code using either Mocha &amp; Chai
                or Jest
              </li>
              <li>
                End to end testing of applications via Cypress
              </li>
            </ul>
            <br />
            <p
              class="d-flex justify-space-between align-center title mt-3 mb-0 pt-10"
            >
              <span>Senior Engineer &amp; Technical Lead</span>
              <span class="body-1">Aug '17 - Apr '18</span>
            </p>
            <p class="d-flex justify-space-between align-center title mb-0">
              <span>Graduate Engineer</span>
              <span class="body-1">Aug '15 - Aug '17</span>
            </p>
            <p class="d-flex justify-space-between align-center title mb-0">
              <span>Undergraduate Engineer</span>
              <span class="body-1">Sep '13 - Sep '14</span>
            </p>
            <v-subheader class="pl-0 mb-2 mt-2 font-italic">
              Weapon Systems Simulation &amp; Experimentation - MBDA
            </v-subheader>
            <p>
              From September 2013 to September 2014 I undertook a year out from
              University at MBDA in the Weapon Systems Simulation &amp;
              Experimentation department, creating distributed simulations of
              production equipment for testing and training purposes.
            </p>
            <p class="pt-2">
              During this time, I developed the departmental intranet and
              maintained C# libraries used for sub-system simulations. At the
              end of my Undergraduate year I was asked to commit to returning as
              a Graduate Engineer pending the successful completion of my final
              year of University.
            </p>
            <p>
              Starting on the Graduate Scheme in August 2015, I worked in
              multiple roles including Developer and Delivery Lead across
              multiple projects; finishing the Graduate scheme as a Senior
              Engineer and the Technical Lead for 2 separate simulation systems.
              I also took courses on Agile Fundamentals, Presentation Skills,
              Negotiation and Project Management.
            </p>
            <ul class="mb-0">
              <li>
                Development of C# software components
              </li>
              <li>
                Led a team of 5+ software engineers on the creation of a complex
                training system within a scrum environment
              </li>
              <li>
                Drove the adoption of web technologies including NodeJS coupled
                with C# &amp; C++ applications to deliver an Instructor Station
                that can run within a web-browser
              </li>
              <li>
                Design authority responsible for system and software
                architectures, sequence diagrams, requirements gathering &amp;
                data exchange specifications/APIs
              </li>
              <li>
                Development of C++ plugins &amp; libraries
              </li>
              <li>
                Co-ordinated a pan-European team of software developers
              </li>
              <li>
                Provided daily reports to Chief Engineers in the run-up to key
                integration events
              </li>
              <li>
                Main point of contact for key stakeholders
              </li>
            </ul>
          </AboutSection>
          <AboutSection title="Personal Interests" icon="mdi-basketball">
            <p>
              Outside of work I enjoy working on my own projects, usually as a
              way to keep up to date on technologies that I do not necessarily
              have the opportunity to work with at my job. For instance, a
              GraphQL Movie API that is a wrapper around The Movie Database REST
              API, and accompanying React frontend. Both projects I undertook so
              as to provide myself an opportunity to work with .NET Core,
              GraphQL &amp; React.
            </p>
            <p>
              I have also developed my own blog using Vue, Vuetify &amp;
              Gridsome, as a way to familiarise myself with static site
              generators, Netlify and JAMStack applications. Prior to that I
              developed my own CMS system using ApolloServer that I deployed to
              DigitalOcean using Docker images automatically built using
              CircleCI and deployed via Kubernetes.
            </p>
            <p>
              I enjoy being involved in team-based sports, having recently
              joined a Cricket club as well as having played Football and
              Basketball from a young age. I spent 2 years as captain of the
              Junior Sharks B Team, 2 years as Captain of the Newcastle
              University Knights &amp; 2 years as President of the Newcastle
              University Knights. I am also a Level 2 Basketball coach and have
              previously coached Basketball to a high level, reaching the
              National League Playoff Finals 3 years running, winning in the 3rd
              year.
            </p>
          </AboutSection>
        </v-col>
      </v-row>
    </v-container>
  </Layout>
</template>

<script>
import AboutSideBar from '../components/AboutSideBar.vue';
import AboutSection from '../components/AboutSection.vue';

export default {
  metaInfo: { title: 'About me' },
  components: { AboutSideBar, AboutSection },
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
}
</style>
