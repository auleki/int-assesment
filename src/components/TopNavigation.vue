<template>
  <div class="top__navigation">
    <div class="search__bar">
      <i class="uil uil-search search__icon icon"></i>
      <input 
        v-model="queryString" 
        class="text__input" 
        type="text" 
        name="queryString" 
        placeholder="Find Something...">
      <button @click="searchPhotos" class="button search">
        <span class="button__text">Search</span>
        <i class="ri-send-plane-line button__icon"></i>
      </button>
    </div>
  
    <div class="nav__actions">
      <i class="ri-notification-3-fill notification__icon"></i>
      <div class="avatar__section">
        <img src="https://www.jesuschristsavior.net/Redeemer.jpeg" alt="" class="avatar">
      </div>
      <div class="user__action">
        <span>Abigail</span>  
        <i class="uil uil-angle-down arrow__icon icon"></i>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'TopNavigation',
    data () {
      return {
        queryString: ''
      }
    },
    methods: {
      searchPhotos () {
        this.queryString = ''
       this.$emit('btn-click')
      }
    }
  }
</script>

<style scoped>
  .top__navigation {
    display: flex;
    align-items: center;
    /* background: blue; */
    
    justify-content: space-between;
    margin-bottom: 3em;
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
  }

  .icon {
    cursor: pointer;
  }

  .notification__icon {
    color: rebeccapurple;
    transition: 200ms ease-in;
  }

  .notification__icon:hover {
    color: gainsboro;
    cursor: pointer;
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
    color: rgb(185, 185, 185);
  }


  .nav__actions {
    margin-left: 1em;
    display: flex;
    align-items: center;
    gap: 1em;
  }

  .arrow__icon, .notification__icon {
    font-size: 2em;
  }

  .text__input {
    padding: 1em;
    outline: 0;
    width: 100%;
    font-size: 1em;
    border: 0;
    color: rebeccapurple;
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
    display: inline-flex;
    top: 1em;
  }

  .button__icon {
    /* display: none; */
    transition: 200ms ease-in-out;
  }

  .button.search > .button__icon {
    transform: rotateZ(0deg);
    /* transform: translateX(100em); */
    /* display: none; */
  }

  .button.search:hover > .button__icon {
    transform: rotateZ(45deg) scale(1.3);
    /* display: inline-flex; */
  }

  .button.search:hover, 
  .button.search:focus  {
    background: #1a1a1a;
    color: gainsboro;
  }

  .user__action {
    align-items: center;
    transition: color 200ms ease-in-out;
    color: rebeccapurple;
    display: flex;
  }

  .user__action:hover {
    cursor: pointer;
    color: gainsboro;
  }
</style>