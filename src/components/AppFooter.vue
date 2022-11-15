<script>
export default {
  name:"AppFooter"
}
</script>

<template>
<footer>
  <div class="top-footer">
    TOP FOOTER
  </div>
  <div class="bottom-footer">
    BOTTOM FOOTER
  </div>

</footer>
</template>


<style lang="scss" scoped>
footer{
  height: 480px;
  .top-footer{
    height: 370px;
    background-color: gray;
    
  }
  .bottom-footer{
    height: 110px;
    background-color: #303030;
  }
}
</style>