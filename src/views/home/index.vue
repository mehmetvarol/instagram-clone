<template>
  <div class="home">
    <div class="time-line"></div>
    <div class="sidebar"></div>
  </div>
</template>

<script>
export default {
  name: 'Home',
  components: {}
}
</script>
<style scoped>
.home {
  max-width: 605px;
  margin-left: auto;
  margin-right: auto;

  @media (--t) {
    max-width: none;
    display: grid;
    grid-template-columns: 1fr 295px;
    grid-gap: 30px;
  }
}
.sidebar {
  display: none;
  @media (--t) {
    display: block;
  }
}
</style>
