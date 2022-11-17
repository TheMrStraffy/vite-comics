<script>
export default {
  name: "AppCard",
  props:{
    comic:Object
  }
}
</script>
<template>
<div class="d-flex justify-content-center col-xl-2 col-lg-3 col-md-4 col-sm-6 col-12">

  <div class="card-mc">
    <div class="card-box">
      <img :src="comic.thumb" alt="comic.series">
      
    </div>
    <div class="text">
      {{comic.series}}
    </div>
  </div>
</div>
</template>


<style lang="scss" scoped>
.card-mc{
  width: 200px;
  height: 240px;
  background-color: none;
  margin-bottom: 20px;
  .card-box{
    height: 190px;
    margin-bottom: 15px;
    img{
      width: 200px;
      height: 190px;
      object-fit: cover;
      object-position: top;
    }
  }
}
</style>