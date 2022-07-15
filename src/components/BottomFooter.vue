<template>
      <div class="low-footer-container py-5">
      <div class="container d-flex justify-content-between align-items-center">
        <a href="#" class="sign-up-btn"> SIGN-UP NOW</a>
        <div class="d-flex align-items-center social-container">
          <span>FOLLOW US</span>
          <a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a>   
          <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a>
          <a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a>
          <a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a>
          <a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a>              
        </div>
      </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
 @import "../styles/variable.scss";
    .low-footer-container{
    background-color: $bottomFooter;

    .sign-up-btn{
      padding: 10px 15px;
      text-decoration: none;
      color:white;
      border: 2px solid $mainColor;
    }

    span{
      color: $mainColor;
      margin-right: 20px;
      font-size: 25px;
    }

    .social-container a{
      margin:0 10px
    }
  }
</style>

