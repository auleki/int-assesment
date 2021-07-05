<template>
  <div class="list__profiles container">    
    <!-- TOP NAVIGATION -->
    <TopNavigation @btn-click="$emit('search-photo')"/>
    <!-- FILTERS -->
    <FilterSelect />
    <!-- PROFILE CARDS -->
    <ProfileCards />
  </div>
</template>

<script>
import ProfileCards from './ProfileCards.vue'
import FilterSelect from './FilterSelect.vue'
import TopNavigation from './TopNavigation.vue'

export default {
  name: 'ListProfiles',
  props: {
    msg: String
  },
  components: {
    ProfileCards,
    FilterSelect, 
    TopNavigation
  }
}
</script>

<style scoped>

  .list__profiles {
    padding: 2em 0 0 1em; 
    overflow-y: scroll;
  }
  
</style>
