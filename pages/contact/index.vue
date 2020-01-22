<template>
  <layout-container>
    <layout-inner>
      <list-tags tags-name="ul">
        <li>ほげほげ</li>
        <li>ほげほげ</li>
        <li>ほげほげ</li>
      </list-tags>
      <base-link name="戻る" path="/" />
      <form-container name="sacss">
        <label for="form-name">名前</label>
        <input id="form-name" name="name" autocomplete="name" type="text" />
        <label for="form-email">メールアドレス</label>
        <input id="form-email" name="email" autocomplete="email" type="email" />
        <label for="form-url">URL</label>
        <input id="form-url" name="url" autocomplete="url" type="url" />
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
    FormContainer,
    ListTags
  }
}
</script>
