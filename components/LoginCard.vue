<template>
  <v-card :width="700" class="card-body">
    <v-card-title>
      <h3 class="page-title">Nuxt Study App</h3>
    </v-card-title>
    <v-card-text>
      <LoginForm @emitLogin="emitLogin" />
    </v-card-text>
  </v-card>
</template>
<script lang="ts">
import { Vue, Component, Emit } from 'nuxt-property-decorator'
@Component
export default class LoginCard extends Vue {
  @Emit('emitLogin')
  emitLogin() {}
}
</script>
<style lang="scss" scoped>
.page-title {
  margin: 30px auto;
}
.card-body {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translateY(-50%) translateX(-50%);
}
</style>
