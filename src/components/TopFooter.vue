<template>
  <div class="top-footer-container">
      <div class="container">
        <div class="row">
          <div class="col-6 py-5 d-flex">
            <div>
                <ul>
                    <h3 class="text-white">DC COMICS</h3>
                    <li v-for="(links,index) in dcComicsList" :key="index">
                        <a :href="links.url"> {{ links.text }}</a>                      
                    </li>
                </ul>
                <ul>
                    <h3 class="text-white">SHOP</h3>
                    <li v-for="(links,index) in shopList" :key="index">
                       <a :href="links.url"> {{ links.text }}</a>  
                    </li>
                </ul>
            </div>
            <div class="px-3">
                  <ul>
                    <h3 class="text-white">DC</h3>
                    <li v-for="(links,index) in dcInfo" :key="index">
                        <a :href="links.url"> {{ links.text }}</a>  
                    </li>
                </ul>
            </div>
            <div>
                  <ul>
                    <h3 class="text-white">SITES</h3>
                    <li v-for="(links,index) in externalSite" :key="index">
                        <a :href="links.url"> {{ links.text }}</a>  
                    </li>
                </ul>
            </div>
          </div>
          <div class="col-6">
            <img class="w-100 position-relative logo-dc-bg" src="../assets/img/dc-logo-bg.png" alt="">
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
    data: function(){
        return{
            dcComicsList:[
                {
                    text:'Characters',
                    url:'#',
                },
                 {
                    text:'Comics',
                    url:'#',
                },
                 {
                    text:'Movies',
                    url:'#',
                },
                 {
                    text:'TV',
                    url:'#',
                },
                 {
                    text:'Games',
                    url:'#',
                },
                {
                    text:'Videos',
                    url:'#',
                },
                {
                    text:'News',
                    url:'#',
                },
            ],
            shopList:[
                {
                    text:'Shop DC',
                    url:'#',
                },
                {
                    text:'Shop DC Collectibles',
                    url:'#',
                }
            ],      
            dcInfo:[
                {
                     text:'Terms Of Use',
                    url:'#',
                },
                {
                     text:'Privacy policy',
                    url:'#',
                },
                {
                     text:'Ad Choices',
                    url:'#',
                },
                {
                     text:'Advertising',
                    url:'#',
                },
                {
                     text:'Jobs',
                    url:'#',
                },
                {
                     text:'Subscriptions',
                    url:'#',
                },
                {
                     text:'Talent Workshops',
                    url:'#',
                },
                {
                     text:'CPSC Certificates',
                    url:'#',
                },
                {
                     text:'Ratings',
                    url:'#',
                },
                {
                     text:'Shop Help',
                    url:'#',
                },
                {
                     text:'Contact Us',
                    url:'#',
                },              
            ],
            externalSite:[
               {
                     text:'DC',
                    url:'#',
                },
                {
                     text:'MAD Magazine',
                    url:'#',
                },
                {
                     text:'DC Kids',
                    url:'#',
                },
                {
                     text:'DC Universe',
                    url:'#',
                },
                {
                     text:'DC Power Visa',
                    url:'#',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    @import "../styles/variable.scss";
    .top-footer-container{
    background-image:url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;
  }

  ul li{
    list-style: none;

    a{
            color: rgb(129, 129, 129);
            text-decoration: none;
    }
  }

  .logo-dc-bg{
    margin:-100px 0;
    z-index: 0;
  }
</style>
