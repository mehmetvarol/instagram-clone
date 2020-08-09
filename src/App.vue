<template>
  <div id="app">
    <MainHeader />
    <main class="main">
      <Container>
        <router-view />
      </Container>
    </main>
  </div>
</template>

<script>
import MainHeader from '@/components/Header'
import Container from '@/components/Container'
export default {
  name: 'App',
  components: {
    Container,
    MainHeader
  }
}
</script>
<style scoped>
.main {
  padding-top: 40px;
}
</style>
