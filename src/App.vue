<template>
  <div id="app">
    <navbar />
    <div id="page-wrapper">
        <router-view/>
    </div>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'

export default {
  components: {
    Navbar
  }
}
</script>

<style>
html {
  height: 100%;
}

body {
  background-color: #cda34f;
  height: 100%;
}

#app {
  height: 100%;
}

#page-wrapper {
    height: calc(100% - 7.5em);
}
</style>
