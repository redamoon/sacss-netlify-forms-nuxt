<template>
  <label :for="name" class="form-label"><slot /></label>
</template>

<script>
export default {
  name: 'FormLabel',
  props: {
    name: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>

</style>
