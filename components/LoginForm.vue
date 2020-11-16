<template>
  <v-form ref="form">
    <v-row class="mx-auto">
      <span class="title-text"> ユーザー名 </span>
      <v-text-field
        placeholder="メールアドレスを入力してください"
        class="input-text"
      />
    </v-row>
    <v-row class="mx-auto">
      <span class="title-text"> パスワード </span>
      <v-text-field class="input-text" />
    </v-row>
    <v-card-actions>
      <v-btn :width="200">ログイン</v-btn>
    </v-card-actions>
  </v-form>
</template>
