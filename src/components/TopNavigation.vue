<template>
  <div class="top__navigation">
    <div class="searchbar">
      <span class="search__icon icon">icon</span>
      <input type="text" name="" id="" placeholder="Find something...">
      <button class="button search">Search</button>
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
  }
</script>

<style scoped>
  .top__navigation {
    display: flex;
    align-items: center;
    justify-content: space-between;
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