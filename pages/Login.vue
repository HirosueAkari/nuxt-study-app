<template>
  <v-container>
    <LoginCard @emitLogin="login" />
  </v-container>
</template>
<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'
@Component
export default class Login extends Vue {
  login() {
    this.$router.push('/home')
  }
}
</script>
