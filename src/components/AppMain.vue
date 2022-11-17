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
    <div class="loadMore d-flex justify-content-center">
      <span>LOAD MORE</span> 
      </div>
</main>
</template>


<style lang="scss" scoped>

main{
  padding: 50px 0;
    background-color: #1c1c1c;
    color: white;
    .container{
      margin-bottom: 20px;
    }
    .loadMore{
      span{
        background-color: #0282f9;
        padding: 10px 30px;
      }
    }
}

</style>