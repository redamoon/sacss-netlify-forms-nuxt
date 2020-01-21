<template>
  <div class="base-link">
    <nuxt-link
      v-if="!disabled"
      :to="path"
      :class="`base-link_button ${className}`"
    >
      {{ name }}
    </nuxt-link>
    <div v-else class="base-link_button -disabled">
      {{ name }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'BaseLink',
  props: {
    name: {
      type: String,
      required: true
    },
    path: {
      type: String,
      required: true
    },
    className: {
      type: String,
      default: '-base'
    },
    disabled: {
      type: Boolean,
      default: false
    }
  }
}
</script>

<style lang="scss" scoped>
.base-link {
  border-radius: 10px;
  display: block;
  &_button {
    &.-disabled {
      opacity: 0.5;
      pointer-events: none;
    }
  }
}
</style>
