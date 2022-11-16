<script>
export default {
  name: "AppCard",
  props:{
    comic:Object
  }
}
</script>
<template>
  <div class="card-mc">
    <div class="card-box">
      <img :src="comic.thumb" alt="comic.series">
      
    </div>
    <div class="text">
      {{comic.series}}
    </div>
  </div>
</template>


<style lang="scss" scoped>
.card-mc{
  width: 200px;
  height: 240px;
  background-color: none;
  .card-box{
    width: 200px;
    height: 190px;
    img{
      width: 200px;
      height: 100%;
      object-fit: cover;
    }
  }
}
</style>