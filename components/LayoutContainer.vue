<template>
  <div class="layout-container">
    <slot />
  </div>
</template>

<script>
export default {
  name: 'LayoutContainer'
}
</script>

<style lang="scss" scoped>
.layout-container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
