<template>
  <v-form ref="form">
    <v-row>
      <span class="title-text"> ユーザー名 </span>
      <v-text-field
        placeholder="メールアドレスを入力してください"
        class="input-text"
      />
    </v-row>
    <v-row>
      <span class="title-text"> パスワード </span>
      <v-text-field class="input-text" />
    </v-row>
    <v-card-actions>
      <v-btn :width="200" class="login-btn" @click="login">ログイン</v-btn>
    </v-card-actions>
  </v-form>
</template>
<script lang="ts">
import { Vue, Component, Emit } from 'nuxt-property-decorator'
@Component
export default class LoginForm extends Vue {
  @Emit('emitLogin')
  login() {}
}
</script>
<style lang="scss" scoped>
.input-text {
  display: inline-block;
}
.title-text {
  display: inline-block;
  font-weight: bold;
  padding-top: 20px;
  margin-right: 16px;
}
.row {
  width: 500px;
  padding-left: 16px;
  margin: 0 auto;
}
.login-btn {
  margin: 20px auto 0;
}
</style>
