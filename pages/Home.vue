<template>
  <strong>home</strong>
</template>
<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'
@Component({
  middleware: 'middleware',
})
export default class Home extends Vue {}
</script>
