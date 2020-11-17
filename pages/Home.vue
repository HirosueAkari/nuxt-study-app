<template>
  <strong>home</strong>
</template>
<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'
@Component({
  middleware: 'middleware',
  layout: 'Logo',
})
export default class Home extends Vue {}
</script>
