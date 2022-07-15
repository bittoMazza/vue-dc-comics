<template>
  <footer>
    <TopFooter/>
    <BottomFooter/>
  </footer>
</template>

<script>
import TopFooter from "./TopFooter.vue"
import BottomFooter from "./BottomFooter.vue"
export default {
  TopFooter,
  BottomFooter,
}
</script>

<style lang="scss" scoped>
@import "../styles/variable.scss";
</style>