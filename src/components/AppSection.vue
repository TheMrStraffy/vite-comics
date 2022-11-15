<script>
export default {
  name:"AppSection",
  data(){
    return{

      images:[
        {
          img: 'buy-comics-digital-comics.png',
          text: 'digital comics',
          link: '#'
        },
        {
          img: 'buy-comics-merchandise.png',
          text: 'dc merchandise',
          link: '#'
        },
        {
          img: 'buy-comics-subscriptions.png',
          text: 'subscription',
          link: '#'
        },
        {
          img: 'buy-comics-shop-locator.png',
          text: 'comic shop locator',
          link: '#'
        },
        {
          img: 'buy-dc-power-visa.svg',
          text: 'dc power visa',
          link: '#'
        },
      ]
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
  <div class="container">
    <div
    v-for="(image,index) in images"
    :key="index"
     class="buyInfos">
      <img :src="getPathImage(image.img)" alt="">
      <a :href="`${image.link}`">{{image.text.toUpperCase()}}</a>
      
    </div>
  </div>
</section>
</template>


<style lang="scss" scoped>
section{
  height: 190px;
  background-color: #0282f9;
}
.container{
  width: 70%;
  height: 100%;
  margin: 0 auto;
  display: flex;
  justify-content: space-evenly;
}
.buyInfos{
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  width: calc(100% / 5);
  img{
    // width: 50%;
    height: 30%;
    
  }
}
a{
  text-decoration: none;
  color: white;

}
</style>