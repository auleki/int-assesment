<template>
  <div class="list__profiles container">
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
    
    <div class="filters">
      <select name="" id="">
        <option>World</option>
        <option value="">eg 2</option>
        <option value="">eg 3</option>
      </select>

      <select name="" id="">
        <option>Following</option>
        <option value="">eg 2</option>
        <option value="">eg 3</option>
      </select>

      <select name="" id="">
        <option>Popular</option>
        <option value="">eg 2</option>
        <option value="">eg 3</option>
      </select>

      <select name="" id="">
        <option>Posts</option>
        <option value="">eg 2</option>
        <option value="">eg 3</option>
      </select>

      <select name="" id="">
        <option>Gender</option>
        <option value="">eg 2</option>
        <option value="">eg 3</option>
      </select>

      <select name="" id="">
        <option>Location</option>
        <option value="">eg 2</option>
        <option value="">eg 3</option>
      </select>

      <select name="" id="">
        <option>Profession</option>
        <option value="">eg 2</option>
        <option value="">eg 3</option>
      </select>

    </div>
    
  </div>
</template>

<script>

export default {
  name: 'ListProfiles',
  props: {
    msg: String
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
