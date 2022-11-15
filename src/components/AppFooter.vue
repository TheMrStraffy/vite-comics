<script>
export default {
  name:"AppFooter",
  data(){
    return{
      dcComicList: [
        { text: 'Characters', link: '#' },
        { text: 'Comics', link: '#' },
        { text: 'Movies', link: '#' },
        { text: 'TV', link: '#' },
        { text: 'Games', link: '#' },
        { text: 'Videos', link: '#' },
        { text: 'News', link: '#' },
      ],
      shopList: [
        {text: 'Shop DC', link: '#'},
        {text: 'Shop DC Collectibles', link: '#'},
      ],
      dcList: [
        { text: 'Terms Of Use', link: '#' },
        { text: 'Privacy policy(New)', link: '#' },
        { text: 'Ad Choices', link: '#' },
        { text: 'Advertising', link: '#' },
        { text: 'Jobs', link: '#' },
        { text: 'Subscriptions', link: '#' },
        { text: 'Talent Workshops', link: '#' },
        { text: 'CPSC Certificates', link: '#' },
        { text: 'Ratings', link: '#' },
        { text: 'Shop Help', link: '#' },
        { text: 'Contact Us', link: '#' },
      ],
      sitesList: [
        {text: 'DC', link: '#'},
        {text: 'MAD Magazine', link: '#'},
        {text: 'DC Kids', link: '#'},
        {text: 'DC Universe', link: '#'},
        {text: 'DC Power Visa', link: '#'},
      ]
    }
  }
}
</script>

<template>
<footer>
  <div class="top-footer">
    <div class="container">
      <div class="left">
        <div class="column">
          <h3>DC COMICS</h3>
          <ul>
            <li
            v-for="(link,index) in dcComicList"
            :key="index"
            ><a :href="link.link">{{link.text}}</a></li>
          </ul>
          <h3>SHOP</h3>
          <ul>
            <li
            v-for="(link,index) in shopList"
            :key="index"
            ><a :href="link.link">{{link.text}}</a></li>
          </ul>
        </div>
        <div class="column">
          <h3>DC</h3>
          <ul>
            <li
            v-for="(link,index) in dcList"
            :key="index"
            ><a :href="link.link">{{link.text}}</a></li>
          </ul>
          
        </div>
        <div class="column">
          <h3>SITES</h3>
          <ul>
            <li
            v-for="(link,index) in sitesList"
            :key="index"
            ><a :href="link.link">{{link.text}}</a></li>
          </ul>
          
        </div>
      </div>
      <div class="right">
      </div>
    </div>
    
  </div>
  <div class="bottom-footer">
    <div class="container">

    BOTTOM FOOTER
    </div>
  </div>

</footer>
</template>


<style lang="scss" scoped>
footer{
  height: 480px;
  .top-footer{
    background-image: url('../img/footer-bg.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: 50% 50%;
    height: 370px;
  }
   
  .bottom-footer{
    height: 110px;
    background-color: #303030;
  }
}
.container{
  width: 70%;
  height: 100%;
  margin: 0 auto;
}
.left{
  padding-top: 40px;
  display: flex;
  // flex-direction: r;
  flex-wrap: wrap;
  h3{
    color: white;
    padding-bottom: 20px;
  }
  .column{
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
</style>