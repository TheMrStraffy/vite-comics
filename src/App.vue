<script>
import AppFooter from './components/AppFooter.vue'
import AppHeader from './components/AppHeader.vue'
import AppJumbotron from './components/AppJumbotron.vue'
import AppMain from './components/AppMain.vue'
import AppSection from './components/AppSection.vue'
export default {
  name: "App",
  
  components: { AppHeader, AppMain, AppFooter, AppSection, AppJumbotron },
}
</script>

<template>
<!-- <div class="container"> -->

<AppHeader/>
<AppJumbotron/>
<AppMain/>
<AppSection/>
<AppFooter/>
<!-- </div> -->
</template>


<style lang="scss">
@use './styles/general.scss' as *;

</style>