<script>
export default {
  name:"AppHeader",
  data(){
    return{
      menu:[
        {
          text: 'characters',
          link: '#',
          current: false
        },
        {
          text: 'comics',
          link: '#',
          current: true
        },
        {
          text: 'movies',
          link: '#',
          current: false
        },
        {
          text: 'tv',
          link: '#',
          current: false
        },
        {
          text: 'games',
          link: '#',
          current: false
        },
        {
          text: 'collectibles',
          link: '#',
          current: false
        },
        {
          text: 'videos',
          link: '#',
          current: false
        },
        {
          text: 'fans',
          link: '#',
          current: false
        },
        {
          text: 'news',
          link: '#',
          current: false
        },
        {
          text: 'shop',
          link: '#',
          current: false
        },
      ]
    }
  }
}
</script>

<template>
<header>
  <div class="container-mc">

  <div class="logo">
    <img src="/dc-logo.png" alt="dc-logo">
  </div>
  <nav>
    <ul>
      <li 
      v-for="(link, index) in menu"
      :key="index"
      >
        <a 
        :class="{'active': link.current}"
        :href="`${link.link}`">{{link.text.toUpperCase()}}</a>
      </li>
    </ul>
  </nav>
  </div>
</header>
</template>


<style lang="scss" scoped>
header{
  height: 120px;
  background-color: white;
  .container-mc{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 70%;
    height: 100%;
    margin: 0 auto;
  }
}
img{
  width: 80px;
}
nav{
  height: 100%;
}
ul{
  display: flex;
  align-items: center;
  height: 100%;
  li{
    list-style-type: none;
    padding: 0px 10px;
    height: 100%;
    a{
      display: flex;
      align-items: center;
      height: 100%;
      text-decoration: none;
      color: #464646;
      &:hover,
      &.active{
        color: #2b82f9;
        border-bottom: 3px solid #2b82f9;
      }
    }
  }
}
</style>