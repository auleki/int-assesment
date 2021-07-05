<template>
  <div class="list__profiles container">    
    <!-- TOP NAVIGATION -->
    <TopNavigation />
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .top__navigation {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .list__profiles {
    padding: 2em 0 0 1em; 
    overflow-y: scroll;
  }

  .avatar__section img {
    height: 75px;
    object-fit: cover;
    width: 75px;
    border-radius: 50%;
    border: .2em solid rgb(219, 219, 219);
  }
  

  .user__action {
    display: flex;
  }
</style>
