<template>
  <div class="home">
    <h1>Profile</h1>
    <CustomText tag="p" size="small">Profile Tag</CustomText>
  </div>
</template>

<script>
import CustomText from '@/components/CustomText'

export default {
  name: 'ProfileTag',
  components: {
    CustomText
  }
}
</script>
