<template>
  <div id="app">
    <Topbar class="topbar" />
    <main>
      <Nav />
      <Content class="content" />
    </main>
  </div>
</template>

<script>
import Topbar from './components/Topbar'
import Nav from './components/Nav'
import Content from './components/Content'

export default {
  name: 'app',
  components: {
    Topbar,Nav,Content
  }
}
</script>

<style lang="scss">
  $borderCor:#e9e9e9; $hoverCor:#108ee9;
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: flex; flex-direction: column; height: 100vh;
  >main{
    margin: 0 2em; flex: 1; background: #fff; border-radius: 5px; padding: 20px 0; display: flex;
    >.content{
      height: 100%; border-left: 1px solid $borderCor; flex: 1; padding-left: 2em; padding-right: 2em;
    }
  }

}

</style>
