<script>
export default {
  name: "AppJumbotron"
}
</script>
<template>
  <div class="jumbotron ">
    <img src="../img/jumbotron.jpg" alt="jumbotron.jpg">
  </div>
</template>


<style lang="scss" scoped>
.jumbotron{
  img{
    width: 100%;
   height: 400px;
   object-fit: cover;
   object-position: top;
 }
}
</style>