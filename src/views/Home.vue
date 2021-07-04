<template>
  <div class="home">
    <Sidebar />
    <ListProfiles />
  </div>
</template>

<script>
// @ is an alias to /src
import ListProfiles from '@/components/ListProfiles.vue'
import Sidebar from '../components/Sidebar.vue'

export default {  
  name: 'Home',
  components: {
    ListProfiles,
    Sidebar
  }
}
</script>

<style scoped>
  .home {
    height: 100vh;
    display: grid;
    grid-template-columns: 20% 80%;
    background: rgb(253, 253, 253);
  }

  
</style>