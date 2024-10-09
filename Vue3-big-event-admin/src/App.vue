<script setup>
import { useRoute, useRouter } from 'vue-router'
const router = useRouter()
const route = useRoute()

const goList = () => {
  router.push('/list')
}
</script>

<template>
  <div>
    I am App
    <button @click="$router.push('/home')">to home</button>
    <button @click="goList">to list</button>
  </div>
</template>

<style scoped></style>
