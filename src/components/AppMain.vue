<script>
import AppSection from './AppSection.vue'
export default {
  components: { AppSection },
  name:"AppMain"
}
</script>

<template>
<main>
  <div class="content">
    CONTENT HERE
  </div>
  <AppSection/>
</main>
</template>


<style lang="scss" scoped>
main{
  height: 290px;
  .content{
    height: 130px;
    background-color: #1c1c1c;
    color: white;
  }
}
</style>