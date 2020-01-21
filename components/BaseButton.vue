<template>
  <button :class="`base-button ${className}`" :type="buttonType">
    {{ name }}
  </button>
</template>

<script>
export default {
  name: 'BaseButton',
  props: {
    name: {
      type: String,
      required: true
    },
    className: {
      type: String,
      default: '-base'
    },
    buttonType: {
      type: String,
      default: 'button'
    }
  }
}
</script>

<style lang="scss" scoped>
.base-button {
  width: 100%;
  padding: 10px;
  border: none;
  border-radius: 10px;
  &.-base {
    color: #FFF;
    background: #3b8070;
  }

  &.-disabled {
    pointer-events: none;
  }
}
</style>
