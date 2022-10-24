<template>
  <NavBar/>
  <ProfileComponent/>
  <DisplayComponent/>
  <AboutComponent/>
  <SkillComponent/>
  <FooterComponent/>
</template>

<script>
import NavBar from './components/NavBar.vue'
import ProfileComponent from './components/ProfileComponent.vue'
import DisplayComponent from './components/DisplayComponent.vue'
import AboutComponent from './components/AboutComponent.vue'
import SkillComponent from './components/SkillComponent.vue'
import FooterComponent from './components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    ProfileComponent,
    DisplayComponent,
    AboutComponent,
    SkillComponent,
    FooterComponent
  }
}
</script>

<style>
#app {
  width: 100%;
  height: 100%;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  position: relative;
  margin: 0;
  padding: 0;
}
</style>
