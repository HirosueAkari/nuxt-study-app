<template>
  <v-card :width="700" class="card-body">
    <v-card-title>
      <h3 class="page-title">Nuxt Study App</h3>
    </v-card-title>
    <v-card-text>
      <LoginForm />
    </v-card-text>
  </v-card>
</template>
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
