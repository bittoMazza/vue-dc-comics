<template>
  <div class="series-card">
    <div href="#" class="container-card-image position-relative" >
        <span class="price-container"> {{ seriesPrice }}</span>
        <img class="card-image" :src="urlImage" :alt="seriesName">
    </div>
    <div>
        <span class="card-title">{{ seriesName }} </span>
    </div>
  </div>
</template>

<script>
export default {
    props:{
        urlImage: String,
        seriesPrice: String,
        seriesName: String,
        seriesType: String,
    }
}
</script>

<style lang="scss" scoped>
@import "../styles/variable.scss";

    .series-card{
        width: calc((100%/ 6) - 30px );
        margin: 0 15px 20px 15px;
        .container-card-image{
            &:hover .price-container{
                display: inline-block;
            }
        }

        .price-container{
            display: none;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%,-50%);
            color: white;
            padding: 5px;
            border-radius: 10px;
            background-color: $mainColor;
            opacity: 0.9;
            font-size: 22px;
        }
        .card-image{
            width:180px;
            height:180px;
            object-fit: cover;     
            object-position: top; 
        }
         .card-title{
            color:white;
            font-size: 12px;
            text-transform: uppercase;
        }
    }

     @media screen and (max-width: 1200px) {
  .series-card{
    width: calc((100% / 4) - 30px);
  }
}
   
</style>

