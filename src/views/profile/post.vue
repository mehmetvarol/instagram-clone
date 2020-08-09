<template>
  <div class="home">
    <h1>Profile</h1>
    <CustomText tag="p" size="small">Profile Post</CustomText>
  </div>
</template>

<script>
import CustomText from '@/components/CustomText'

export default {
  name: 'ProfilePost',
  components: {
    CustomText
  }
}
</script>
