<script>
export default {
  name: "AppJumbotron"
}
</script>
<template>
  <div class="jumbotron ">
    <img src="../img/jumbotron.jpg" alt="jumbotron.jpg">
    <div class="currentSeries">
      CURRENT SERIES
    </div>
  </div>
</template>


<style lang="scss" scoped>
.jumbotron{
  position: relative;
  img{
    width: 100%;
   height: 400px;
   object-fit: cover;
   object-position: top;
 }
  .currentSeries{
    position: absolute;
    bottom: -5%;
    left: 10%;
    font-size: 1.3rem;
    font-weight: 600;
    background-color: #0282f9;
    color: white;
    padding: 10px 25px;
  }
}
</style>