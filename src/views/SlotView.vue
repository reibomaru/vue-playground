<template>
  <div>
    <p>スロット</p>
    <custom-padding>
      <template #content="contentProps">
        {{ contentProps.msg }}
      </template>
    </custom-padding>
  </div>
</template>

<script lang="ts">
export default {
  name: 'SlotView'
}
</script>

<script lang="ts" setup>
import CustomPadding from '@/components/Padding.vue'
</script>
