<script setup lang="ts">
import { ref } from 'vue'
import SideBarManu from './components/SideBarMenu.vue'

const message = ref('Hello Padel Point User')
</script>

<template>
  <h1>{{ message }}</h1>
  <SideBarManu />
</template>

<style scoped></style>
