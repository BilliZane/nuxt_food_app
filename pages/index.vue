<template>
  <main class="container">
    <AppHeader />
    <AppRestaurantInfo />
  </main>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue'
import AppRestaurantInfo from '@/components/AppRestaurantInfo.vue'

export default {
  head () {
    return {
      title: 'Home'
    }
  },

  components: {
    AppHeader,
    AppRestaurantInfo
  }
}
</script>
