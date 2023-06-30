<template>
  <main class="container">
    <AppHeader />
    <AppRestaurantInfo :dataSource="fooddata"/>
  </main>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue'
import AppRestaurantInfo from '@/components/AppRestaurantInfo.vue'
import { mapState } from 'vuex'

export default {
  head () {
    return {
      title: 'Home'
    }
  },

  computed: {
    ...mapState(['fooddata'])
  },

  components: {
    AppHeader,
    AppRestaurantInfo
  }
}
</script>
