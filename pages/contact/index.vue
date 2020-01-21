<template>
  <layout-container>
    <layout-inner>
      <base-link name="戻る" path="/" />
    </layout-inner>
  </layout-container>
</template>

<script>
import LayoutContainer from '~/components/LayoutContainer'
import LayoutInner from '~/components/LayoutInner'
import BaseLink from '~/components/BaseLink'

export default {
  components: {
    LayoutContainer,
    LayoutInner,
    BaseLink
  }
}
</script>
