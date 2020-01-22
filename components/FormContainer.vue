<template>
  <form :name="name" method="POST" data-netlify="true" class="form-container">
    <slot />
  </form>
</template>

<script>
export default {
  name: 'FormContainer',
  props: {
    name: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
.form-container {
  width: 100%;
}
</style>
