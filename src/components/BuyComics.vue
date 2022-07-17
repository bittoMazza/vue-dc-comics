<template>
  <div class="buy-comics">
            <div class="container d-flex justify-content-between align-items-center px-5">
                <div v-for="(buyLink,index) in buyComics" :key="index">
                    <img class="logos-buy-comics" :src="buyLink.urlImg" alt="">
                    <a href="#" class="text-white text-decoration-none"> {{ buyLink.text }}</a>
                </div>
            </div>           
        </div>
</template>

<script>
export default {
    data: function(){
        return{
            buyComics:[
                {
                    text:'DIGITAL COMICS',
                    urlImg:'http://localhost:8080/img/buy-comics-digital-comics.png',
                },
                {
                    text:'DC MERCHANDISE',
                    urlImg:'http://localhost:8080/img/buy-comics-merchandise.png',
                },
                {
                    text:'SUBSCRIPTION',
                    urlImg:'http://localhost:8080/img/buy-comics-shop-locator.png',
                },
                {
                    text:'COMIC SHOP LOCATOR',
                    urlImg:'http://localhost:8080/img/buy-comics-subscriptions.png',
                },
                {
                    text:'DC POWER VISA',
                    urlImg:'http://localhost:8080/img/buy-dc-power-visa.svg',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../styles/variable.scss";
     .buy-comics{
        padding: 50px 0;
        background-color: $mainColor;
    }
    .logos-buy-comics{
        height: 40px;
        margin-right: 10px;
    }
</style>