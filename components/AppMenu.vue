<template>
  <nav>
    <ul>
      <li>
        <nuxt-link exact to="/"><AppLogo /></nuxt-link>
      </li>
      <li><nuxt-link to="restaurants">Restaurants</nuxt-link></li>
    </ul>
    <nuxt-link to="/cart">Cart</nuxt-link>
  </nav>
</template>

<script>
import NuxtLogo from './NuxtLogo.vue'
import AppLogo from './AppLogo.vue'

export default {
  components: {
    NuxtLogo,
    AppLogo
  }
}
</script>
