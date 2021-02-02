<template>
  <figure class="avatar">
    <img :src="src" :alt="alt" :height="size" :width="size" />
  </figure>
</template>

<script>
export default {
  name: 'Avatar',
  props: {
    src: {
      type: String,
      default:
        'https://www.gravatar.com/avatar/205e460b479e2e5b48aec07710c08d50'
    },
    alt: {
      type: String
    },
    size: {
      type: Number
    }
  }
}
</script>

<style scoped>
.avatar {
  display: inline-flex;
  padding: 2px;
  border-radius: 999px;
  background: linear-gradient(
    219deg,
    rgba(184, 63, 140, 1) 0%,
    rgba(237, 158, 90, 1) 100%
  );
  img {
    border-radius: inherit;
    border: 2px solid white;
  }
}
</style>
