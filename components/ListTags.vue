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
    return createElement(this.tagsName, this.$slots.default)
  }
}
</script>
