<template>
  <nav>
    <ul>
      <li>
        <nuxt-link exact to="/"><AppLogo /></nuxt-link>
      </li>
      <li>
        <nuxt-link to="restaurants" v-if="!showRestItem">Restaurants</nuxt-link>
      </li>
    </ul>
    <div class="smallnum" v-if="cartCount > 0">{{ cartCount }}</div>
    <nuxt-link to="/cart">Cart</nuxt-link>
  </nav>
</template>

<script>
import NuxtLogo from './NuxtLogo.vue'
import AppLogo from './AppLogo.vue'
import { mapGetters } from 'vuex'

export default {
  components: {
    NuxtLogo,
    AppLogo
  },

  computed: {
    showRestItem () {
      return (
        this.$route.path.includes('cart') ||
        this.$route.path.includes('items') ||
        this.$route.path.includes('restaurants')
      )
    },

    ...mapGetters(['cartCount'])
  }
}
</script>
