<template>
  <div id="app">
    <div id="nav">
      <Nav />
    </div>

    <router-view />

  </div>
</template>

<script>
import Nav from './components/Nav'
export default {
  name: "app",
  components: {
    Nav
  }
}
</script>

<style>

</style>
