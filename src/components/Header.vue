<template>
  <header>
    <div class="container-fluid">
      <!-- logo -->
      <div class="logo">
        <img src="../assets/dark-logo.png" alt="logo">
      </div>
      <!-- nav centrale -->
      <div class="main-nav">
        <ul>
          <li v-for="(list, index) in listHeader" :key="index">{{list.item}}<i class="fas fa-chevron-down"></i></li>
        </ul>
      </div>
      <!-- nav dx -->
      <div class="right-nav">
        <ul>
          <li>
            <img :src=flagPath alt="language-flag">
            <!-- :src="require(`../assets/${flagPath}`)" -->
          </li>
          <li>
            <select name="language" @change="selectedLang(lang)" v-model="lang">
              <option v-for="(list, index) in listHeaderRight" :key="index">{{list.language}}</option>
            </select>
          </li>   
          <li>
            <i class="far fa-user-circle"></i>
          </li>
          <li>
            <form>
              <div class="input-group">
                <input type="text" class="form-control" placeholder="Search...">
              </div>
              <button type="submit" class="btn btn-outline-secondary" @click.prevent><i class="fas fa-search"></i></button>
            </form>
          </li>       
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: {
    listHeader: Array,
    listHeaderRight: Array
  },
  data: function() {
    return {
      selected: "",
      lang: ""
    }
  },
  methods: {
    selectedLang: function(lang) {
      this.selected = lang;
      console.log(this.selected);
    }
  },
  computed: {
    flagPath: function() {
      let newFlag = "";
      if (this.selected == "ENGLISH") {
        newFlag = require(`../assets/en.png`)
      } else if (this.selected == "FRENCH") {
        newFlag = require(`../assets/fr.png`)
      } else if (this.selected == "GERMAN") {
        newFlag = require(`../assets/de.png`)
      }
      return newFlag;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/mixins.scss';
 
 header {
   color: $darkSilver;
   @include ul-clean;

   .container-fluid {
    height: 80px;
    @include flex;
   }

   .logo img {
     width: 150px;
     margin-left: 150px;
   }

    ul {
    @include flex; 
    @include ul-clean;

      & li i{
        font-size: 10px;
        padding-left: 4px;
      }
    }

    .main-nav {
      li {
        padding-left: 24px;
      }
    }

    .right-nav {

      color: $darkSilver;
      margin-left: 10px;

      img {
        width: 28px;
      }

      select {
        border: 0px;
        &:hover {
          cursor: pointer;
        }
      }

      li {
        padding-left: 6px;
      }

      i {
        font-size: 16px;
      }

      form {
        @include flex;
        border-left: 1px solid $silver;
        height: 80px;
        
        input,
        button {
          border: 0px;
        }

      }
    }


 }
</style>
