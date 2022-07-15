<template>
    <main>
        <div class="content-container container py-5">
            <h2 class="text-white fs-5"> -- > CONTENT GOES HERE   -- </h2>
        </div>
        <div class="buy-comics">
            <div class="container d-flex justify-content-between">
                <div v-for="(buyLink,index) in buyComics" :key="index">
                    <img class="logos-buy-comics" :src="buyLink.url" alt="">
                    <span> {{ buyLink.text }}</span>
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
                    url:'../assets/img/buy-comics-digital-comics.png',
                },
                 {
                    text:'DC MERCHANDISE',
                    url:'../assets/img/buy-comics-digital-comics.png'
                },
                 {
                    text:'SUBSCRIPTION',
                    url:'../assets/img/buy-comics-digital-comics.png'
                },
                 {
                    text:'COMIC SHOP LOCATOR',
                    url:'../assets/img/buy-comics-digital-comics.png'
                },
                 {
                    text:'DC POWER VISA',
                    url:''
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
        background-color: $mainColor;
    }
    .logos-buy-comics{
        width: 30px;
    }
</style>
