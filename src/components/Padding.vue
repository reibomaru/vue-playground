<template>
  <div class="container">
    <slot name="content" msg="hoge"></slot>
  </div>
</template>

<script lang="ts">
export default {
  name: 'CustomPadding'
}
</script>

<script lang="ts" setup>
import { defineSlots } from 'vue'
defineSlots<{
  content(props: { msg: string }): any
}>()
</script>
<style lang="scss">
.container {
  padding: 40px;
  background-color: black;
}
</style>
