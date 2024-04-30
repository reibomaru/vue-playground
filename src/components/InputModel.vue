<template>
  <div>
    <div>{{ label }}: {{ input }}</div>
    <input type="text" v-model="input" placeholder="ここに何かを入力" />
  </div>
</template>
<script lang="ts">
export default {
  name: 'InputModel'
}
</script>

<script lang="ts" setup>
import { defineModel } from 'vue'
defineProps<{
  label: string
}>()
const input = defineModel({ required: true })
</script>
