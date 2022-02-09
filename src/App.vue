<template>
  <div id="app">
    <Header />
    <nav-bar/>
    <main-box/>
    <exellence-and-innovation/>
    <class-facilities/>
    <events/>
    <news/>
    <join-us/>
    <footer-box/>
    <social-s/>
  </div>
</template>

<script>
import ClassFacilities from './components/ClassFacilities.vue'
import Events from './components/Events.vue'
import ExellenceAndInnovation from './components/ExellenceAndInnovation.vue'
import Header from './components/Header.vue'
import JoinUs from './components/JoinUs.vue'
import MainBox from './components/MainBox.vue'
import FooterBox from './components/FooterBox.vue'
import NavBar from './components/NavBar.vue'
import News from './components/News.vue'
import SocialS from './components/SocialS.vue'


export default {
  name: 'App',
  components: {
    Header,
    NavBar,
    MainBox,
    ExellenceAndInnovation,
    ClassFacilities,
    Events,
    News,
    JoinUs,
    FooterBox,
    SocialS,
  }
}
</script>
    JoinUsript>
   

<style lang="css">

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}
</style>
