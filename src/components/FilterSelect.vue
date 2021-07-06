<template>
  <div class="filters">
      <select class="select__input" name="" id="">
        <option>World</option>
        <option value="">eg 2</option>
        <option value="">eg 3</option>
      </select>

      <select class="select__input" name="" id="">
        <option>Following</option>
        <option value="">eg 2</option>
        <option value="">eg 3</option>
      </select>

      <select class="select__input" name="" id="">
        <option>Popular</option>
        <option value="">eg 2</option>
        <option value="">eg 3</option>
      </select>

      <select class="select__input" name="" id="">
        <option>Posts</option>
        <option value="">eg 2</option>
        <option value="">eg 3</option>
      </select>

      <select class="select__input" name="" id="">
        <option>Gender</option>
        <option value="">eg 2</option>
        <option value="">eg 3</option>
      </select>

      <select class="select__input" name="" id="">
        <option>Location</option>
        <option value="">eg 2</option>
        <option value="">eg 3</option>
      </select>

      <select class="select__input" name="" id="">
        <option>Profession</option>
        <option value="">eg 2</option>
        <option value="">eg 3</option>
      </select>
    </div>
</template>

<script>
  export default {
    name: 'FilterSelect'
  }

</script>

<style scoped>
  .filters {
    /* background: rebeccapurple; */
    justify-content: center;
    display: flex;
    border-radius: .3em;
    /* border: 1px solid black; */
    overflow: hidden;
    padding-right: 1em;
  }

  .select__input {
    border: 0;
    outline: 0;
    border-right: .1em solid gainsboro;
    padding: 1.5em;
    width: 100%;
    /* color:#fff; */
    text-align: center;
    /* background: rgb(65, 65, 65); */
    background: #fff;
  }


</style>
/* <!-- -->  */
