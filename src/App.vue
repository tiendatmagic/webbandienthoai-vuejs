<template>
  <div id="app">
<Menu/>
<List/>
<Footer/>
  </div>
</template>

<script>

import Menu from './components/Menu'
import List from './components/List'
import Footer from './components/Footer'
export default {

  components: {

    Menu,
    List,
    Footer
  }
}
</script>

<style>
* {
  margin: 0px;
  padding: 0px;
}

</style>
