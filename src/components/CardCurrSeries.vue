<template>
  <div class="series-card">
    <a href="#" class="container-card-image" >
        <img class="card-image" :src="urlImage" :alt="seriesName">
    </a>
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
    .series-card{
        width: calc((100%/ 6) - 30px );
        margin: 0 15px 20px 15px;
        .card-image{
            width: 100%;
            padding-bottom: 10px;
        }
         .card-title{
            color:white;
            font-size: 12px;
            text-transform: uppercase;
        }
    }
   
</style>

