<template>
  <from :name="name" method="POST" data-netlify="true" class="from-container">
    <slot />
  </from>
</template>

<script>
export default {
  name: 'FromContainer',
  props: {
    name: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
.from-container {
  width: 100%;
}
</style>
