<template>
  <header class="header">
    <Container class="header-inner">
      <router-link to="/" class="logo">
        İnstagram
      </router-link>
      <form class="search">
        <input type="text" placeholder="Serach..." />
      </form>
      <nav class="navigation">
        <router-link to="/">
          <IconHomeFill v-if="$route.name === 'Home'" />
          <IconHome v-else />
        </router-link>
        <router-link to="/direct">
          <IconDirectFill v-if="$route.name === 'Direct'" />
          <IconDirect v-else />
        </router-link>
        <router-link to="/explore">
          <IconExploreFill v-if="$route.name === 'Explore'" />
          <IconExplore v-else />
        </router-link>
        <router-link to="/profile">Profile</router-link>
      </nav>
    </Container>
  </header>
</template>

<script>
import Container from '@/components/Container'
import IconHome from '@/assets/icons/home.svg'
import IconHomeFill from '@/assets/icons/home-fill.svg'
import IconDirect from '@/assets/icons/direct.svg'
import IconDirectFill from '@/assets/icons/direct-fill.svg'
import IconExplore from '@/assets/icons/explore.svg'
import IconExploreFill from '@/assets/icons/explore-fill.svg'

export default {
  name: 'MainHeader',
  components: {
    Container,
    IconHome,
    IconHomeFill,
    IconDirect,
    IconDirectFill,
    IconExplore,
    IconExploreFill
  }
}
</script>
<style scoped>
.header {
  position: fixed;
  left: 0;
  right: 0;
  top: 0;
  z-index: 90;
  border-bottom: 1px solid rgb(var(--b6a));
}
.header-inner {
  height: 60px;
  display: flex;
  justify-content: center;
  align-items: center;

  @media (--t) {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    align-items: center;
  }
}
.logo {
  font-size: 1.6rem;
  font-weight: bold;
  text-decoration: none;
}
.search {
  display: none;

  @media (--t) {
    display: block;
    text-align: center;

    input {
      width: 215px;
      height: 28px;
      border: 1px solid rgb(var(--b6a));
      background-color: rgb(var(--b3f));
      border-radius: 4px;
      padding-left: 20px;
      padding-right: 20px;
    }
  }
  text-align: center;

  input {
    width: 215px;
    height: 28px;
    border: 1px solid rgb(var(--b6a));
    background-color: rgb(var(--b3f));
    border-radius: 4px;
    padding-left: 20px;
    padding-right: 20px;
  }
}
.navigation {
  z-index: 90;
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #fff;
  height: 120px;
  display: flex;
  align-items: center;
  justify-content: space-around;

  @media (--t) {
    height: auto;
    position: static;
    justify-content: flex-end;
    border: 0;
    a {
      margin-left: 20px;
    }
  }
}
</style>
