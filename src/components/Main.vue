<template>
    <main>
        <CurrentSeries/>
        <BuyComics/>
    </main>
</template>

<script>
import BuyComics from "./BuyComics.vue";
import CurrentSeries from "./CurrentSeries.vue"
export default {
    components:{
        BuyComics,
        CurrentSeries,
    }
}
</script>

<style lang="scss">
@import "../styles/variable.scss";
      main{
        position: relative;
        z-index: 1;
    }
</style>
