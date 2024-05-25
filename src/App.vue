<template>
  <Header />

  <About />
  <News />
  <Publications />
  <Education />
  <Academic />
  <Award />
  <Work />
  <Interests />
  <Friends />

</template>

<script>
import Header from './components/Header.vue'
import About from './components/About.vue'
import Publications from './components/Publications.vue';
import Education from './components/Education.vue';
import Academic from './components/Academic.vue';
import Award from './components/Award.vue';
import Work from './components/Work.vue';
import Interests from './components/Interests.vue';
import Friends from './components/Friends.vue';
import News from './components/News.vue';

export default {
  components: {
    Header, About, Publications, Education, Academic, Award, Work, Interests, Friends, News
  }
}
</script>