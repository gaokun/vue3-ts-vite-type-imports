<script setup lang="ts">
// import type { MsgProps } from './msg' // OK
import type { MsgProps } from './types'  // NG

defineProps<MsgProps>()
</script>

<template>
  <h1>{{ msg }}</h1>
</template>
