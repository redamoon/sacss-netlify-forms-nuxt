<template>
  <div class="layout-inner">
    <slot />
  </div>
</template>

<script>
export default {
  name: 'LayoutInner'
}
</script>

<style lang="scss" scoped>
.layout-inner {
  padding: 20px;
}
</style>
