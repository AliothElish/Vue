<script setup>
import { useRoute, useRouter } from 'vue-router'
import { useUserStore, useCountStore } from '@/stores'

const router = useRouter()
const route = useRoute()

const goList = () => {
  router.push('/list')
  console.log(router, route)
}

const userStore = useUserStore()
const countStore = useCountStore()
</script>

<template>
  <div>
    I am App
    <test-demo></test-demo>
    <el-button @click="$router.push('/home')">Jump to home page</el-button>
    <el-button @click="goList">Jump to list page</el-button>

    <el-button type="primary">Primary</el-button>
    <el-button type="success">Success</el-button>

    <p>{{ userStore.token }}</p>
    <el-button @click="userStore.setToken('Bearer sidfhheiwhuvyweqrjh')">
      Log in
    </el-button>
    <el-button @click="userStore.removeToken()">quit</el-button>

    <hr />
    {{ countStore.count }}
    <el-button @click="userStore.add(2)">addition</el-button>
  </div>
</template>

<style scoped></style>
