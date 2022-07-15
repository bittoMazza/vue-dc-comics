<template>
  <header>
    <div class="d-flex justify-content-between align-items-center nav-container py-4 container">
      <img class="header-logo" src="../assets/img/dc-logo.png" alt="Logo dc">
      <nav>
        <ul>
          <li v-for="(links,index) in headerLinkList" :key="index">
            {{ links.text }}
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  data:function(){
    return{
      headerLinkList:[
        {
          text: "CHARACTERS",
          url: "#"
        },
        {
          text: "COMICS",
          url: "#"
        },
        {
          text: "MOVIES",
          url: "#"
        },
        {
          text: "TV",
          url: "#"
        },
        {
          text: "GAMES",
          url: "#"
        },
        {
          text: "COLLECTIBILES",
          url: "#"
        },
        {
          text: "VIDEOS",
          url: "#"
        },
        {
          text: "FANS",
          url: "#"
        },
        {
          text: "NEWS",
          url: "#"
        },
        {
          text: "SHOP",
          url: "#"
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../styles/variable.scss";
    nav ul{
    li{
      display: inline-block;
      padding: 10px;
      font-weight: bold;
      font-size: 14px;
    }
  }

  .header-logo{
    height: 80px;
  }

</style>>

