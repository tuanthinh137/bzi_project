<template>
  <div class="wrapper">
    <Header />
    <div class="container container--full">
      <div class="f main">
        <SideBar />
        <Content />
      </div>
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import SideBar from './components/SideBar.vue'
import Content from './components/Content.vue'
import '../src/assets/css/style.css'

export default {
  name: 'App',
  components: {
    Header,
    SideBar,
    Content
  }
}
</script>
