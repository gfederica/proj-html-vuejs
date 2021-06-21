<template>
  <div id="app">
    <Header :listHeader="this.headerList" :listHeaderRight="this.headerRight"/>
  </div>
</template>

<script>

import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header
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
                langFlag: require('./assets/images/en.png'),
                language: "ENGLISH"
              },
              {
                langFlag: require('./assets/images/de.png'),
                language: "GERMAN"
              },
              {
                langFlag: require('./assets/images/fr.png'),
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
