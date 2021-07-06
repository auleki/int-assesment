<template>
  <section class="profile__card">
    <div class="profile__image">
      <img src="https://coolmenshair.com/wp-content/uploads/interlocking-dreadlocks-14.jpg" alt="" srcset="">
    </div>
    <div class="profile__info">
      <h3 class="user__information">Mary J Blige, 28</h3>
      <div class="extra__info">
        <div class="profile__location center__y">
          <i class="ri-map-pin-5-fill"></i>
          <span class="location">New York</span>
        </div>
        <div class="profile__actions center">
          <button class="button like__profile">
            <i class="ri-heart-2-line"></i>
          </button>
          <button class="button dislike__profile">
            <i class="ri-thumb-down-line"></i>
          </button>
        </div>
      </div>
      
    </div>
  </section>
</template>

<script>
  export default {
    name: 'ProfileCard'
  }
</script>

<style scoped>
  .profile__card {
    background: transparent;
    /* background: rgb(73, 73, 73); */
    color: #fff;
    border-radius: .3em;
    position: relative;
    height: 100%;
    overflow: hidden;
    width: 100%;
  }

  .profile__info, 
  .profile__actions, 
  .user__information,
  .profile__locations {
    margin: .5em 0;
  }

  .extra__info {
    padding: .5em 1em;
    position: absolute;
    height: 50%;
    z-index: 1;
    background: transparent;
    width: 100%;
    transition: 250ms ease-in-out;
    bottom: -1em;
    color: #1a1a1a;
    left: 0;
  }

  .profile__card > .extra__info {
    /* opacity: 0; */
  }

  .profile__card:hover > .extra__info {
    background: white;
    opacity: 1;
    bottom: -1em;
  }

  .like__profile, .dislike__profile {
    width: 100%;
  }

  .like__profile {
    background: red;
    color: #fff;
  }

  .dislike__profile {
    background: rebeccapurple;
    color: #fff;
  }

  .like__profile:hover, .dislike__profile:hover {
    background: rgb(224, 224, 224);
    color: #333;
  }

  .profile__actions {
    display: flex;
    gap: 2em;
  }
  
  .profile__image img {
    height: 25em;
    object-fit: cover;
    width: 25em;
    border-radius: .3em;
  } 
</style>