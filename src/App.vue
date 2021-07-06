<template>
  <!-- <div id="nav">
    <router-link to="/">Home</router-link> 
  </div> -->
  <router-view/>
</template>

<style>
  * {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }

  body {
    font-family: Arial, Helvetica, sans-serif;
  }

  .center, 
  .center__y, 
  .center__x {
    display: flex;
  }

  .center {
    justify-content: center;
    align-items: center;
  }

  .center__x {
    justify-content: center;
  }

  .center__y {
    align-items: center;
  }

  .button {
    padding: 1em 2em;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: .5em;
    outline: 0;
    transition: 200ms ease-in;
    font-size: 1em;
    border-radius: .3em;
    border: 0; 
  }

  .button:hover {
    cursor: pointer;
    background: #333;
    color: #fff
  }
</style>