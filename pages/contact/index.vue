<template>
  <layout-container>
    <layout-inner>
      <el-card class="box-card login">
        <base-link name="戻る" path="/" />
      </el-card>
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
