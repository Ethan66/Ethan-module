<template>
  <div id="app">
    <Topbar />
    <main>
      <Nav />
    </main>
  </div>
</template>

<script>
import Topbar from './components/Topbar'
import Nav from './components/Nav'

export default {
  name: 'app',
  components: {
    Topbar,Nav
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
  main{
    margin: 0 4em;
  }
</style>
