<template>
    <main>
        <div class="content-container container py-5">
            <h2 class="text-white fs-5"> -- > CONTENT GOES HERE   -- </h2>
        </div>
        <BuyComics/>
    </main>
</template>

<script>
import BuyComics from "./BuyComics.vue";
export default {
    components:{
        BuyComics,
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
</style>
