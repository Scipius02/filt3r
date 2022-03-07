<template>
  <div>
    <SiteHeader />
    <main>
      <MainLayout />
    </main>
    <SiteFooter />
  </div>
</template>

<script>
import SiteHeader from './components/SiteHeader.vue';
import SiteFooter from './components/SiteFooter.vue';
import MainLayout from './components/MainLayout.vue';

export default {
  name: 'App',
  components: {
    SiteHeader,
    SiteFooter,
    MainLayout,
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: #2c3e50;
  color:antiquewhite;
}

@import "./styles/bootstrap.css";

</style>
