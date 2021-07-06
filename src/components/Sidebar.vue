<template>
  <div class="sidebar">
    <!-- replace with proper link element -->
    <div class="sidenav__logo">
      <h1>LOGO</h1>
    </div>
    
    <div class="sidebar__links">
      <section class="sidenav__link active">
        <!-- <span class="icon"><i class="lni lni-home"></i></span> -->
        <i class="uil uil-home icon"></i>
        <span class="link__text">Home</span>      
      </section>

      <section class="sidenav__link">
        <!-- <span class="icon">H</span> -->
        <i class="uil uil-comment-add icon"></i>
        <span class="link__text">Messages</span>    
      </section>
    </div>

    <div class="sidenav__title">
      <h4>SHARE</h4>
    </div>

    <div class="sidebar__links">
      <section class="sidenav__link">
        <!-- <span class="icon">H</span> -->
        <i class="uil uil-chart icon"></i>
        <span class="link__text">Ranking</span>    
      </section>

      <section class="sidenav__link">
        <i class="uil uil-dollar-alt icon"></i>
        <span class="link__text">Challenge</span>    
      </section>

      <section class="sidenav__link">
        <!-- <span class="icon">H</span> -->
        <!-- <i class="uil uil-chart"></i> -->
        <i class="uil uil-megaphone icon"></i>
        <span class="link__text">Party</span>    
      </section>

      <section class="sidenav__link">
        <!-- <span class="icon">H</span> -->
        <i class="uil uil-link icon"></i>
        <span class="link__text">Connect</span>    
      </section>

      <section class="sidenav__link">
        <!-- <span class="icon">H</span> -->
        <i class="uil uil-fidget-spinner icon"></i>
        <span class="link__text">Parade</span>   
      </section>

      <section class="sidenav__link">
        <!-- <span class="icon">H</span> -->
        <i class="uil uil-users-alt icon"></i>
        <span class="link__text">Group</span>    
      </section>

    </div>
  </div>
</template>

<style scoped>
  .sidebar {
    border-right: .2em solid rgb(238, 238, 238);
    padding: 2em 1em 0 1em; 
    overflow: hidden;
  }

  .sidenav__links {
    display: flex;
    flex-direction: column;
    gap: .5em;
  }

  .sidenav__logo {
    margin-bottom: 3em;
  }

  .sidenav__link {
    display: flex;
    gap: .5em;
    color: rgb(121, 121, 121);
    border-radius: .3em;
    padding: 1em;
    border: .2em solid transparent;
  }

  .icon {
    font-size: 1;
    display: inline-block;
    transition: 250ms ease-in;
  }

  .icon:hover {
    transform: scale(2);
  }

  .sidenav__link:hover {
    cursor: pointer;
    color: black;
  }

  .link__text, .icon {
    transition: 200ms ease-out;
  }

  .sidenav__link:hover > .link__text {
    transform: translateX(.3em);
  }

  .sidenav__link:hover > .icon {
    color: rebeccapurple;
    transform: scale(1.3);
  }

  .sidenav__link:not(:last-child) {
     margin-bottom: .5em;
  }

  .sidenav__link.active {
    color: #1a1a1a;
    border-color: gainsboro;
  }

  .sidenav__link.active:hover {
    /* color: rebeccapurple; */
    color: #fff;
    background: rgb(209, 209, 209);
    border-color: transparent;
  }

  .sidenav__link.active:hover > .icon {
    color: #fff;
  }

  .sidenav__title {
    margin: 1em 0;
    padding: 1em;
  }



</style>