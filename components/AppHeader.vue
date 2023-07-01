<template>
  <section class="header" role="img" aria-label="Image Description">
    <h1 class="header__title">Nuxt Food App</h1>
    <nuxt-link to="/restaurants">
      <button class="header__btn">See restaurants</button>
    </nuxt-link>
  </section>
</template>

<style lang="scss" scoped>
.header {
  width: 100%;
  height: 80vh;
  padding: 40px;
  overflow: hidden;
  background-size: cover !important;
  background: radial-gradient(
      ellipse at center,
      rgba(0, 0, 0, 0) 0%,
      rgba(0, 0, 0, 0) 37%,
      rgba(0, 0, 0, 0.65) 100%
    ),
    url('@/assets/headerimg.jpg') no-repeat center center scroll;

  &__title {
    font-style: normal;
    font-weight: bold;
    color: #eee;
    font-size: 8vmin;
    letter-spacing: 0.03em;
    line-height: 1;
    text-shadow: 1px 2px 4px rgba(0, 0, 0, 0.8);
    margin-bottom: 40px;
  }
}
</style>
