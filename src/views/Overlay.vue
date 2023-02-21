<template>
  <section class="overlay">
    <nav>
      <h4>CrunchyROLL</h4>
      <ul>
        <li>Anime List</li>
        <li>Nominees</li>
        <li>2021 Recap</li>
      </ul>
      <h5>Menu</h5>
    </nav>
    <div class="overlay__text">
      <h1>Crunchyroll</h1>
      <h1 class="sub">Anime Recap — 2022</h1>
    </div>
    <footer class="overlay__footer">
      <h5>[scroll down]</h5>
      <h5>[©2022 - All right reserved]</h5>
    </footer>
  </section>
</template>

<script lang="ts" setup></script>

<style scoped lang="scss">
.overlay {
  position: absolute;
  z-index: 2;
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  nav {
    @extend %flex-ac-jb;
    padding: 3rem 1.5rem 1.5rem;
    height: 7vh;
    h4,
    h5,
    li {
      font-family: "Swansea", sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: Max(1rem, 16px);
      line-height: 150%;
      letter-spacing: 0.02em;
      text-transform: capitalize;
      color: #f3f3f3;
    }
    ul {
      @extend %flex-ac;
      gap: 1rem;
    }
  }
  &__text {
    width: Min(1045px, 100%);
    margin: 6.3rem auto 0;
    h1 {
      font-family: "Melodrama", sans-serif;
      font-style: normal;
      font-weight: 500;
      font-size: 172px;
      line-height: 100%;
      letter-spacing: -0.02em;
      color: #f3f3f3;
      &.sub {
        text-align: right;
      }
    }
  }
  &__footer {
    position: fixed;
    height: 4vh;
    @extend %flex-ac;
    gap: 10rem;
    bottom: 3rem;
    left: 1.5rem;
    h5 {
      font-family: "Swansea", sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: Max(1rem, 16px);
      line-height: 150%;
      letter-spacing: 0.02em;
      text-transform: capitalize;
      color: #f3f3f3;
    }
  }
}
</style>
