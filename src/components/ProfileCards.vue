<template>
  <section class="profile__cards">
    <ProfileCard />
    <ProfileCard />
    <ProfileCard />
    <ProfileCard />
    <ProfileCard />
    <ProfileCard />
    <ProfileCard />
  </section >
</template>

<script>
import ProfileCard from './ProfileCard.vue'

  export default {
    name: 'ProfileCards',
    components: {
      ProfileCard
    },
    props: {
      images: Array
    }
  }
</script>

<style scoped>
  .profile__cards {
    display: grid;
    margin-top: 3em;
    gap: 1em;
    grid-template-columns: repeat(5, 1fr);
  }
</style>