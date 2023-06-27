<template>
  <main class="mcontainer restaurant">
    <div class="restaurantheading">
      <h1>Restaurants</h1>
    </div>

    <AppRestaurantInfo />
  </main>
</template>

<script>
import AppRestaurantInfo from '@/components/AppRestaurantInfo.vue'

export default {
  head () {
    return {
      title: 'Restaurants'
    }
  },

  components: {
    AppRestaurantInfo
  }
}
</script>
