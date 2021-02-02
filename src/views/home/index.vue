<template>
  <div class="home">
    <div class="timeline">
      <Post />
    </div>

    <div class="sidebar">
      <CustomText>lorem</CustomText>
    </div>
  </div>
</template>

<script>
import CustomText from '@/components/CustomText'
import Post from '@/components/Post'

export default {
  name: 'Home',
  components: {
    Post,
    CustomText
  }
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
