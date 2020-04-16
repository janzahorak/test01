<template>
  <div id="app">
    <Navigation />
    <Hero />
    <Section
      title="Section title"
      perex="Lorem ipsum dolor sit amet"
    >
      <Grid1 />
    </Section>
    <section-full-width>
      <Grid2 />
    </section-full-width>
    <Section
      :title="'Section title something'"
      :perex="'Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet'"
      :layout-reverse="true"
    >
      <Grid1 />
    </Section>
    <Section
      :title="'Menu'"
      >
        <Menu />
    </Section>
  </div>
</template>

<script>
import Navigation from './components/Navigation.vue'
import Hero from './components/Hero.vue'
import Section from './components/Section.vue'
import SectionFullWidth from './components/SectionFullWidth.vue'
import Grid1 from './components/grid1.vue'
import Grid2 from './components/grid2.vue'
import Menu from './components/menu.vue'

export default {
  name: 'App',
  components: {
    Navigation,
    Hero,
    Section,
    Grid1,
    Grid2,
    SectionFullWidth,
    Menu
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

section {
  margin: 40px 0;
}
</style>
