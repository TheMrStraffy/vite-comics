<script>
export default {
  name:"AppFooter"
}
</script>

<template>
<footer>
  <div class="top-footer">
    <div class="container">
      TOP FOOTER
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
</style>