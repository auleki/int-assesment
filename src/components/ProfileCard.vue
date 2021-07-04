<template>
  <section class="profile__card">
    <div class="profile__image">
      <img src="https://www.cheatsheet.com/wp-content/uploads/2021/06/Mary-J.-Blige.jpg" alt="" srcset="">
    </div>
    <div class="profile__info">
      <h3 class="user__information">Mary J Blige, 28</h3>
      <div class="profile__location">
        <span class="location__icon">PIN</span>
        <span class="location">New York</span>
      </div>
      <div class="profile__actions">
        <button class="button like__profile">Like</button>
        <button class="button dislike__profile">Unlike</button>
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
    /* background: transparent; */
    background: rgb(93, 182, 255);
    color: #fff;
    border-radius: .3em;
    height: 100%;
    width: 20em;
  }

  .profile__info {
    padding: .5em 1em;
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


  /* .dislike__profile:hover {
    background
  } */

  .profile__actions {
    display: flex;
    justify-content: space-evenly;
  }
  
  .profile__image img {
    height: 100%;
    object-fit: cover;
    width: 100%;
    border-radius: .3em;
  } 
</style>