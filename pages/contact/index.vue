<template>
  <layout-container>
    <layout-inner>
      <base-link name="戻る" path="/" />
      <form-container name="sacss">
        <label for="form-name">名前</label>
        <input id="form-name" name="name" type="text" />
        <label for="form-email">メールアドレス</label>
        <input id="form-email" name="email" type="email" />
        <label for="form-url">URL</label>
        <input id="form-url" name="url" type="url" />
        <button type="submit">送信</button>
      </form-container>
    </layout-inner>
  </layout-container>
</template>

<script>
import LayoutContainer from '~/components/LayoutContainer'
import LayoutInner from '~/components/LayoutInner'
import BaseLink from '~/components/BaseLink'
import FormContainer from '~/components/FormContainer'
import ListTags from '~/components/ListTags'

export default {
  components: {
    LayoutContainer,
    LayoutInner,
    BaseLink,
    FormContainer
  }
}
</script>

<style>
li {
  text-align: left;
}
</style>
