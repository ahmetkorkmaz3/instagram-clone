<template>
  <div class="home">
    <h1>Home</h1>
    <CustomText tag="p">Hello</CustomText>
    <CustomText tag="b" size="x-small">Hello</CustomText>
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
