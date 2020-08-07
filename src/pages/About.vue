<template>
  <Layout>
    <div class="sections">
      <Name />
      <Experience />
      <Agile />
      <Process />
    </div>
  </Layout>
</template>

<script>
import { onMounted } from '@vue/composition-api';
import { setMeta } from '../set-meta';
import AOS from 'aos';
import 'aos/dist/aos.css';

import Name from '../components/about-sections/Name.vue';
import Experience from '../components/about-sections/Experience.vue';
import Agile from '../components/about-sections/Agile.vue';
import Process from '../components/about-sections/Process.vue';

export default {
  components: { Name, Experience, Agile, Process },
  metaInfo() {
    return setMeta(
      'About me & my software development experience',
      'I (Matt Law) am a software developer in Nottingham (UK). I specialise in Web Technologies such as .NET Core, C#, JavaScript, VueJS, HTML & CSS. I also have experience as a system architect and have worked with a variety of cloud providers such as Azure, AWS & Google Firebase.',
      [],
      '/about'
    );
  },
  setup() {
    onMounted(() =>
      AOS.init({
        anchorPlacement: 'bottom-bottom',
      })
    );
    return {};
  },
};
</script>

<style lang="scss" scoped>
.sections {
  &::v-deep {
    .container,
    .row {
      min-height: 100vh;
    }

    p,
    ul {
      font-weight: bold;
      font-size: 2rem;
      line-height: 2.5rem;
      margin: 0;
    }

    ul {
      list-style-type: none;

      li {
        margin: 5px 0;

        &:after {
          content: '-';
          position: absolute;
          right: -20px;
          top: 0;
        }
      }
    }

    h3 {
      font-size: 2.5rem;
      line-height: 2.7rem;
      margin: 20px 0;
    }

    p {
      &.subtitle {
        text-shadow: 1px 1px 1px var(--v-accent-base),
          2px 2px 1px var(--v-accent-base);

        font-size: 2.5rem;
        line-height: 2.7rem;
      }
    }

    .avatar {
      border-radius: 500px;
      border: 10px solid var(--v-primary-base);
    }
  }
}
</style>
