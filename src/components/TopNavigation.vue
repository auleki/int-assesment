<template>
  <div class="top__navigation">
    <div class="search__bar">
      <i class="lni lni-search-alt search__icon icon"></i>
      <input 
        v-model="queryString" 
        class="text__input" 
        type="text" 
        name="queryString" 
        placeholder="Find Something...">
      <button @click="searchPhotos" class="button search">Search</button>
    </div>
    <span class="bell__icon icon">bell</span>
    <div class="avatar__section">
      <img src="https://www.jesuschristsavior.net/Redeemer.jpeg" alt="" class="avatar">
    </div>
    <div class="user__action">
      <span>Abigail</span>
      <span class="dropdown__icon">^</span>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'TopNavigation',
    data () {
      return {
        queryString: 'Monkey own banana'
      }
    },
    methods: {
      searchPhotos () {
       this.$emit('btn-click')
      }
    }
  }
</script>

<style scoped>
  .top__navigation {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .search__bar {
    background: rgb(255, 255, 255);
    width: 100%;
    display: flex;    
    padding: 1em 0 1em 1em;
    border-radius: .3em;
    align-items: center;
    border: .1em solid rgb(230, 230, 230);
    position: relative;
    box-shadow: -2px -1px 24px -2px rgba(70, 70, 70, 0.18);
    margin-bottom: 3em;
  }

  .avatar__section img {
    height: 75px;
    object-fit: cover;
    width: 75px;
    border-radius: 50%;
    border: .2em solid rgb(219, 219, 219);
  }

  .search__icon {
    font-size: 2em;
    /* font-weight: 600; */
    color: rgb(185, 185, 185);
  }

  .text__input {
    padding: 1em;
    outline: 0;
    width: 100%;
    font-size: 1em;
    border: 0;
    background: transparent;
  }

  .text__input::placeholder {
    color: gainsboro;
  }

  .button.search {
    background: rgb(46, 19, 201);
    color: #fff;
    position: absolute;
    right: 1em;
    top: 1em;
  }

  .user__action {
    display: flex;
  }
</style>