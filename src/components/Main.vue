<template>
    <main>
        <div class="content-container container py-5">
            <h2 class="text-white fs-5"> -- > CONTENT GOES HERE   -- </h2>
        </div>
        <div class="buy-comics">
            <div class="container d-flex justify-content-between align-items-center">
                <div v-for="(buyLink,index) in buyComics" :key="index">
                    <img class="logos-buy-comics" :src="buyLink.urlImg" alt="">
                    <span class="text-white"> {{ buyLink.text }}</span>
                </div>
            </div>           
        </div>
    </main>
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
      main{
        position: relative;
        z-index: 1;
        background-color: black;
    }
    .buy-comics{
        padding: 50px 0;
        background-color: $mainColor;
    }
    .logos-buy-comics{
        height: 50px;
        margin-right: 10px;
    }
</style>
