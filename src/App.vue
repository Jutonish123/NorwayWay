<template>
  <Header />
  <router-view/>
</template>

<script>

import Header from './components/Header'

export default {
  components: {
    Header
  }
}
</script>
<style lang="sass">

@import './assets/style/style'

#app
  font-family: 'Nunito', sans-serif
  text-align: center
</style>
