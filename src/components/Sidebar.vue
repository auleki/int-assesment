<template>
  <div class="sidebar">
    <!-- replace with proper link element -->
    <div class="sidebar__links">
      <section class="sidenav__link active">
        <span class="icon">H</span>
        <span class="link__text">Home</span>    
      </section>

      <section class="sidenav__link">
        <span class="icon">H</span>
        <span class="link__text">Messages</span>    
      </section>
    </div>

    <div class="sidenav__title">
      <h4>SHARE</h4>
    </div>

    <div class="sidebar__links">
      <section class="sidenav__link">
        <span class="icon">H</span>
        <span class="link__text">Ranking</span>    
      </section>

      <section class="sidenav__link">
        <span class="icon">H</span>
        <span class="link__text">Challenge</span>    
      </section>

      <section class="sidenav__link">
        <span class="icon">H</span>
        <span class="link__text">Party</span>    
      </section>

      <section class="sidenav__link">
        <span class="icon">H</span>
        <span class="link__text">Connect</span>    
      </section>

      <section class="sidenav__link">
        <span class="icon">H</span>
        <span class="link__text">Parade</span>    
      </section>

      <section class="sidenav__link">
        <span class="icon">H</span>
        <span class="link__text">Group</span>    
      </section>

    </div>
  </div>
</template>

<style scoped>
  .sidebar {
    border-right: .2em solid rgb(238, 238, 238);
    padding: 2em 1em 0 1em; 
  }

  .sidenav__links {
    display: flex;
    flex-direction: column;
    gap: 1em;
  }

  .sidenav__link {
    display: flex;
    gap: .5em;
    color: rgb(121, 121, 121);
    border-radius: .3em;
    padding: 1em;
    border: .2em solid transparent;
  }

  .sidenav__link:hover {
    cursor: pointer;
    color: black;
  }

  .sidenav__link:not(:last-child) {
     margin-bottom: 1em;
  }

  .sidenav__link.active {
    color: black;
    border-color: gainsboro;
  }

  .sidenav__title {
    margin: 1em 0;
    padding: 1em;
  }



</style>