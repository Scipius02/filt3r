<template>
  <main>
    <TextView />
  </main>
  <!-- this will be the template to describe how to organise views as a grid on the page -->
</template>

<script>
  import TextView from "./TextView.vue";

  export default {
    name: "MainLayout",
    components: {TextView}
  }
</script>

<style>
  .main {
    display: flex;
  }
  
</style>