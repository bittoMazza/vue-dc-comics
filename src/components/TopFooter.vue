<template>
  <div class="top-footer-container">
      <div class="container">
        <div class="row">
          <div class="col-6 py-5 d-flex">
            <div>
                <ul>
                    <h3 class="text-white">DC COMICS</h3>
                    <li v-for="(links,index) in dcComicsList" :key="index">
                        <a href=""> {{ links.text }}</a>                      
                    </li>
                </ul>
                <ul>
                    <h3 class="text-white">SHOP</h3>
                    <li v-for="(links,index) in shopList" :key="index">
                       <a href=""> {{ links.text }}</a>  
                    </li>
                </ul>
            </div>
            <div class="px-3">
                  <ul>
                    <h3 class="text-white">DC</h3>
                    <li v-for="(links,index) in dcInfo" :key="index">
                        <a href=""> {{ links.text }}</a>  
                    </li>
                </ul>
            </div>
            <div>
                  <ul>
                    <h3 class="text-white">SITES</h3>
                    <li v-for="(links,index) in externalSite" :key="index">
                        <a href=""> {{ links.text }}</a>  
                    </li>
                </ul>
            </div>
          </div>
          <div class="col-6">
            <img class="position-relative logo-pa" src="../assets/img/dc-logo-bg.png" alt="">
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
                    text:'Characters',
                    url:'#',
                },
                 {
                    text:'Characters',
                    url:'#',
                },
                 {
                    text:'Characters',
                    url:'#',
                },
                {
                    text:'Characters',
                    url:'#',
                },
                {
                    text:'Characters',
                    url:'#',
                },
            ],
            shopList:[
                {
                    text:'Shop DC',
                    url:'#',
                },
                {
                    text:'Characters',
                    url:'#',
                }
            ],      
            dcInfo:[
                {
                     text:'Terms Of Use',
                    url:'#',
                },
                {
                     text:'Characters',
                    url:'#',
                },
                {
                     text:'Characters',
                    url:'#',
                },
                {
                     text:'Characters',
                    url:'#',
                },
                {
                     text:'Characters',
                    url:'#',
                },
                {
                     text:'Characters',
                    url:'#',
                },
                {
                     text:'Characters',
                    url:'#',
                },
                {
                     text:'Characters',
                    url:'#',
                },
                {
                     text:'Characters',
                    url:'#',
                },
                {
                     text:'Characters',
                    url:'#',
                },
                {
                     text:'Characters',
                    url:'#',
                },              
            ],
            externalSite:[
               {
                     text:'DC',
                    url:'#',
                },
                {
                     text:'Characters',
                    url:'#',
                },
                {
                     text:'Characters',
                    url:'#',
                },
                {
                     text:'Characters',
                    url:'#',
                },
                {
                     text:'Characters',
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

  .logo-pa{
    margin:-50px 0;
    z-index: 0;
  }
</style>
