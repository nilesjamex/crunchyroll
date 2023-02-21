<template>
  <section class="home">
    <div class="home__img">
      <img
        src="https://res.cloudinary.com/dx9pt4ggx/image/upload/v1676987534/armin_hglwnh.png"
        alt="A picture of armin, an attack on titan character"
        height="540"
        width="357"
        class="armin"
      />
      <img
        src="https://res.cloudinary.com/dx9pt4ggx/image/upload/v1676987541/wolf_cxvkxp.png"
        alt="A wolf"
        height="371"
        width="300"
        class="wolf"
      />
    </div>
    <Overlay />
  </section>
</template>

<script lang="ts" setup>
import Overlay from "./Overlay.vue";
</script>

<style scoped lang="scss">
.home {
  height: 100vh;
  width: 100vw;
  position: relative;
  overflow: hidden;
  &__img {
    position: absolute;
    z-index: 1;
    height: 100vh;
    width: 100vw;
    padding-top: 8rem;
    .wolf {
      position: absolute;
      bottom: 0;
      right: 10%;
    }
    .armin {
      position: absolute;
      left: 20%;
      top: 20%;
    }
  }
}
</style>
