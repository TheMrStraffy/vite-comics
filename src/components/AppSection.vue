<script>
import imageDB from '../data/imageDB';
export default {
  name:"AppSection",
  data(){
    return{
      imageDB
    }
  },
  methods:{
    getPathImage(imageName){
      return new URL(`../img/${imageName}`, import.meta.url).href
    }
  },
}
</script>

<template>
<section>
  <div class="container py-5">
    <div class="row justify-content-between align-items-center">

      <div
        v-for="(image,index) in imageDB.images"
        :key="index"
        class="buyInfos col-lg-2 d-flex align-items-center justify-content-center">
        <img :src="getPathImage(image.img)" alt="">
        <a :href="`${image.link}`">{{image.text.toUpperCase()}}</a>
      </div>
    </div>
  </div>
</section>
</template>


<style lang="scss" scoped>
section{ 
  background-color: #0282f9;
}
.buyInfos{
  padding: 20px 0;
}
img{
  height: 100px;
}
a{
  margin-left: 5px;
  text-decoration: none;
  color: white;
}
</style>