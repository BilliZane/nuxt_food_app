<template>
  <section class="header" role="img" aria-label="Image Description">
    <h1 class="header__title">Nuxt Food App</h1>
    <button class="header__btn">See restaurants</button>
  </section>
</template>

<script>
export default {}
</script>

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

  &__btn {
    background: #098191;
    transition: background ease 0.25s;
    border-radius: 5px;
    display: inline-block;
    border: none;
    padding: 0.75rem 1.5rem;
    margin: 0;
    text-decoration: none;
    color: #ffffff;
    font-size: 1.2rem;
    cursor: pointer;
    text-align: center;
  }
  &__btn:hover {
    background: #63b6b8;
  }
  &__btn:focus {
    outline: 1px solid #fff;
    outline-offset: -4px;
  }
}
</style>
