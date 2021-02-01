<template>
  <component :is="tag" :class="size">
    <slot />
  </component>
</template>

<script>
export default {
  name: 'CustomText',
  props: {
    tag: {
      type: String,
      default: 'span'
    },
    size: {
      type: String,
      default: 'normal',
      validator: function(value) {
        return ['normal', 'small', 'x-small', 'xx-small'].indexOf(value) !== -1
      }
    }
  }
}
</script>

<style scoped>
.small {
  font-size: 12px;
}

.x-small {
  font-size: 11px;
}

.xx-small {
  font-size: 10px;
}
</style>
