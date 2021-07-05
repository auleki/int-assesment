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

  .button {
    padding: 1em 2em;
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