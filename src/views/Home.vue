<template>
  <div class="home">
    <h1>Home</h1>
    <CustomText tag="p" size="small">Mehmet VAROL</CustomText>
    <IconHome />
  </div>
</template>

<script>
import CustomText from '@/components/CustomText'
import IconHome from '@/assets/icons/home.svg'
export default {
  name: 'Home',
  components: {
    CustomText,
    IconHome
  }
}
</script>
