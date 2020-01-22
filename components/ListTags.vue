<script>
export default {
  name: 'ListTags',
  props: {
    tagsName: {
      type: String,
      required: true
    }
  },
  render(createElement) {
    const tag = this.tagsName
    return createElement(
      tag,
      {
        attrs: {
          class: 'list-tags -' + tag
        }
      },
      this.$slots.default
    )
  }
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
