<template>
  <v-container>
    <LoginCard @emitLogin="login" />
    {{ data }}
  </v-container>
</template>
<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'
@Component
export default class Login extends Vue {
  login() {
    this.$router.push('/home')
  }

  async asyncData({ app }: any) {
    const { data } = await app.$axios.get(
      'https://jsonplaceholder.typicode.com/users'
    )
    return { data: data[0] }
  }
}
</script>
