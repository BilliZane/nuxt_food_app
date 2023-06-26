<template>
  <nav>
    <ul>
      <li><nuxt-link exact to="/">Home</nuxt-link></li>
      <li><nuxt-link exact to="restaurants">Restaurants</nuxt-link></li>
    </ul>
  </nav>
</template>

<script>
import NuxtLogo from './NuxtLogo.vue'
export default {
  components: { NuxtLogo }
}
</script>
