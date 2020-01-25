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
        <p>満足度</p>
        <list-tags tags-name="ul">
          <li>
            <label for="form-good">参加してよかった</label>
            <input
              id="form-good"
              name="form-satisfaction"
              type="radio"
              value="参加してよかった"
            />
          </li>
          <li>
            <label for="form-usually">普通</label>
            <input
              id="form-usually"
              name="form-satisfaction"
              type="radio"
              value="普通"
            />
          </li>
          <li>
            <label for="form-not-good">良くなかった</label>
            <input
              id="form-not-good"
              name="form-satisfaction"
              type="radio"
              value="楽しくなかった"
            />
          </li>
        </list-tags>
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

<style>
li {
  text-align: left;
}
</style>
