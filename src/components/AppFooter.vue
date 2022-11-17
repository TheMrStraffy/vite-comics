<script>
import footerMenuList from '../data/footerMenuList';
export default {
  name:"AppFooter",
  data(){
    return{
      footerMenuList
    }
  }
}
</script>

<template>
<footer>
  <div class="top-footer">
    <div class="container">
      <div class="left">
        <div class="column-mc">
          <h5>DC COMICS</h5>
          <ul class="p-0">
            <li
            v-for="(link,index) in footerMenuList.dcComicList"
            :key="index"
            ><a :href="link.link">{{link.text}}</a></li>
          </ul>
          <h5>SHOP</h5>
          <ul class="p-0">
            <li
            v-for="(link,index) in footerMenuList.shopList"
            :key="index"
            ><a :href="link.link">{{link.text}}</a></li>
          </ul>
        </div>
        <div class="column-mc">
          <h5>DC</h5>
          <ul class="p-0">
            <li
            v-for="(link,index) in footerMenuList.dcList"
            :key="index"
            ><a :href="link.link">{{link.text}}</a></li>
          </ul>
          
        </div>
        <div class="column-mc">
          <h5>SITES</h5>
          <ul class="p-0">
            <li
            v-for="(link,index) in footerMenuList.sitesList"
            :key="index"
            ><a :href="link.link">{{link.text}}</a></li>
          </ul>
          
        </div>
      </div>
    </div>
    
  </div>
  <div class="bottom-footer">
    <div class="container d-flex justify-content-between align-content-center h-100">
      <div class="signUp">

      <button>SIGN-UP NOW!</button>
      </div>

      <div class="socials">
        <span>FOLLOW US</span>
        <img src="../img/footer-facebook.png" alt="">
        <img src="../img/footer-periscope.png" alt="">
        <img src="../img/footer-pinterest.png" alt="">
        <img src="../img/footer-twitter.png" alt="">
        <img src="../img/footer-youtube.png" alt="">
      </div>
    
    </div>
  </div>

</footer>
</template>


<style lang="scss" scoped>
footer{
  // height: 480px;
  .top-footer{
    background-image: url('../img/footer-bg.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: 50% 50%;
    // height: 370px;
    .container{
      background-image: url('../img/dc-logo-bg.png');
      background-repeat: no-repeat;
      position: relative;
      background-position: right;
    }
  }
   
  .bottom-footer{
    height: 110px;
    background-color: #303030;
    .container{
      align-items: center;
    }
  }
}
// .container{
//   width: 70%;
//   height: 100%;
//   margin: 0 auto;
//   display: flex;
//   justify-content: space-between;
// }
.left{
  padding-top: 20px;
  display: flex;
  flex-wrap: wrap;
  h5{
    color: white;
    padding-bottom: 10px;
  }
  .column-mc{
    margin-right: 25px;
  }
}
li{
  list-style-type: none;
  margin-bottom: 5px;
  a{
    text-decoration: none;
    color: #959595;
  }
}
.right{
  width: 40%;
  .img-box{
      // position: relative;
      width: 100%;
      height: 100%;
      overflow: hidden;
    img{
      // position: absolute;
      width: 100%;
      height: 100%;
      // top: -20%;
  }
  }
}
button{
  height: 50px;
  padding: 10px;
  color: white;
  background-color: #303030;
  border-color:#0282f9;
}
.socials{

  span{
    color: #0282f9;
  }
}
</style>