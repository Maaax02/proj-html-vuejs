<template>
  <div id="app">
    <Header />
    <nav-bar/>
    <main-box/>
    <exellence-and-innovation/>
    <class-facilities/>
  </div>
</template>

<script>
import ClassFacilities from './components/ClassFacilities.vue'
import ExellenceAndInnovation from './components/ExellenceAndInnovation.vue'
import Header from './components/Header.vue'
import MainBox from './components/MainBox.vue'
import NavBar from './components/NavBar.vue'

export default {
  name: 'App',
  components: {
    Header,
    NavBar,
    MainBox,
    ExellenceAndInnovation,
    ClassFacilities
  }
}
</script>
   

<style lang="css">

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}
</style>
