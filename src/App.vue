<template>
  <div class="site">
    <div class="nav">
      <div class="home">
        <!-- TODO: Add wolf SVG here but make sure it ends up at 100px x 100px @ 1080p (scaled up or down based on viewport) -->
      </div>
      <div class="box1">
        <p>About</p>
      </div>
      <div class="box2">
        <p>Crafts</p>
      </div>
      <div class="box3">
        <p>Programs</p>
      </div>
      <div class="box4">
        <p>Social</p>
      </div>      
    </div>
    <div class="content">
      <div class="namebox">
        <div class="name" />
      </div>
    </div>
  </div>
</template>

<script>
//import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {

  },
};
</script>

<style scoped>

  .site {
    display: grid;
    grid-area: inherit;
    grid-template-columns: 1fr;
    grid-template-rows: 48px 1fr;
    grid-template-areas: 
      "nav"
      "content"
    ;
    width: 100vw;
    height: 100vh;
  }
    .nav {
      grid-area: nav;
      display: grid;
      grid-template-columns: 48px 1fr 2fr 1fr 2fr 1fr 2fr 1fr 2fr 1fr 48px;
      grid-template-rows: 1fr;
      grid-template-areas: 
        "wolf . box1 . box2 . box3 . box4 ."
      ;
      background: #330851;
    }

      p {
        color: #F5D5E0;
        font-family: Work Sans;
        font-style: normal;
        font-weight: normal;
        font-size: 64px;
        line-height: 75px;
        display: flex;
        align-items: center;
        text-align: center;
      }

      .home {
        grid-area: wolf;
        background: coral;
      }

      .box1 {
        grid-area: box1;
        background: red;
      }

      .box2 {
        grid-area: box2;
        background: red;
      }

      .box3 {
        grid-area: box3;
        background: red;
      }

      .box4 {
        grid-area: box4;
        background: red;
      }

    .content {
      grid-area: content;

      background: #210535;
    }

</style>
