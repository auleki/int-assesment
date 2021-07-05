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

// https://api.unsplash.com/photos/?client_id=YOUR_ACCESS_KEY

export default {  
  name: 'Home',
  methods: {
    async fetchPictures () {
      try {
        const res = await fetch(`${this.url}?client_id=${this.accessKey}`)
        const data = await res.json()
        return data
      } catch (error) {
        console.log(error)
      }
    }
  },
  async created () {
    const fetchedImages = await this.fetchPictures()
    this.images = fetchedImages
    console.log(fetchedImages)
  },
  data () {
    return {
      images: [],
      accessKey: 'ZbZuYQFCAiv5ajdrojf-hnGAK5hNRpjU0hIlK-fbJcE',
      url: 'https://api.unsplash.com/photos'
    }
  },
  components: {
    ListProfiles,
    Sidebar
  }
}
</script>

<style scoped>
  .home {
    height: 100vh;
    overflow-y: hidden;
    display: grid;
    grid-template-columns: 15% 85%;
    background: rgb(248, 248, 248);
  }
</style>