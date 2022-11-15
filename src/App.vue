<script>
import AppFooter from './components/AppFooter.vue'
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppSection from './components/AppSection.vue'

export default {
  name: "App",
  components: { AppHeader, AppMain, AppFooter, AppSection },
}
</script>

<template>
<div class="container">

<AppHeader/>
<AppMain/>
<AppSection/>
<AppFooter/>
</div>
</template>


<style lang="scss">
@use './styles/general.scss' as *;
.container{
  height: 100vh;
}
</style>