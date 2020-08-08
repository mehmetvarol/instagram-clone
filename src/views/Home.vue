<template>
  <div class="home">
    <h1>Home</h1>
    <CustomText tag="p" size="small">Mehmet VAROL</CustomText>
  </div>
</template>

<script>
import CustomText from '@/components/CustomText'
export default {
  name: 'Home',
  components: {
    CustomText
  }
}
</script>
