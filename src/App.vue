<template>
  <div id="app">
    <Header :listHeader="this.headerList" :listHeaderRight="this.headerRight"/>
    <Jumbotron/>
    <Together/>
    <Explore/>
    <Video/>
    <Upcoming/>
    <Footer/>

  </div>
</template>

<script>

import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Jumbotron from './components/Jumbotron.vue'
import Together from './components/Together.vue'
import Explore from './components/Explore.vue'
import Video from './components/Video.vue'
import Upcoming from './components/Upcoming.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Jumbotron,
    Together,
    Explore,
    Video,
    Upcoming
  },
  data: function() {
        return {
            headerList: [
              {
                item: "Home",
                active: false
              },
              {
                item: "Pages",
                active: false
              },
              {
                item: "Courses",
                active: false
              },
              {
                item: "Features",
                active: false
              },
              {
                item: "Blog",
                active: false
              },
              {
                item: "Shop",
                active: false
              }
            ],
            headerRight : [
              {
                langFlag: "en.png",
                language: "ENGLISH"
              },
              {
                langFlag: "de.png",
                language: "GERMAN"
              },
              {
                langFlag: "fr.png",
                language: "FRENCH"
              }
            ]
        }
    }
}
</script>

<style lang="scss">
@import '~bootstrap/scss/bootstrap';
@import './style/general.scss';
@import './style/mixins.scss';
@import '~@fortawesome/fontawesome-free/css/all.min.css';

#app {
  font-family: 'Poppins', sans-serif;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
