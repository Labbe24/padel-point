<script setup lang="ts">
import { ref } from 'vue'
import SideBarManu from './components/SideBarMenu.vue'

const message = ref('Hello Padel Point User')
</script>

<template>
  <v-layout class="rounded rounded-md">
    <v-app-bar title="Padel Point" />

    <SideBarManu />

    <v-main class="d-flex align-center justify-center" style="min-height: 300px">
      Main Content
    </v-main>
  </v-layout>
</template>

<style scoped></style>
