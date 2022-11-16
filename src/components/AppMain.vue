<script>
import AppCardVue from './AppCard.vue'
import catalogue from '../data/catalogue'
export default {
  components: {AppCardVue},
  name:"AppMain",
  data(){
    return{
      catalogue
    }
  }
}
</script>

<template>
<main>
  <div class="container d-flex ">
    <div class="row m-auto justify-content-evenly">
      <AppCardVue 
      v-for="(item, index) in catalogue" :key="index" :comic="item"/>
     
    </div>
  </div>
</main>
</template>


<style lang="scss" scoped>

main{
  padding: 50px 0;
    background-color: #1c1c1c;
    color: white;
}

</style>