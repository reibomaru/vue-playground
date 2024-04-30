<template>
  <div>
    <input-model label="入力" v-model="input" />
    Parent Value: {{ input }}
  </div>
</template>
<script lang="ts">
export default {
  name: 'InputView'
}
</script>

<script lang="ts" setup>
import InputModel from '@/components/InputModel.vue'
import { ref } from 'vue'
const input = ref('')
</script>
