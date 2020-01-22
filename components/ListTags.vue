<template>
  <component :is="elementTags(tagsName)" :class="`list-tags -${tagsName}`">
    <slot />
  </component>
</template>

<script>
export default {
  name: 'ListTags',
  props: {
    tagsName: {
      type: String,
      required: true
    }
  },
  methods: {
    elementTags(tag) {
      return tag
    }
  }
  // render(createElement) {
  //   return createElement(
  //     this.tagsName,
  //     { class: 'list-tags -' + this.TagsName },
  //     this.$slots.default
  //   )
  // }
}
</script>

<style lang="scss" scoped>
.list-tags {
  &.-ol {
    color: #ff4500;
  }
  &.-ul {
    color: #3b8070;
  }
}
</style>
