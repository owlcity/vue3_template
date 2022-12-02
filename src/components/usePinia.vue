<template>
  <div>{{ userStore.name }}</div>
</template>

<script setup>
import { useUserStore } from '@/store/user'

const userStore = useUserStore()
console.log(userStore)
userStore.updateName('李四')
</script>