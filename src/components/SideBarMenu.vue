<script setup lang="ts">
import { ref } from 'vue'

const drawer = ref(true)
const rail = ref(true)
</script>

<template>
  <v-card>
    <v-layout>
      <v-navigation-drawer v-model="drawer" :rail="rail" permanent @click="rail = false">
        <v-list-item
          prepend-avatar="https://randomuser.me/api/portraits/men/85.jpg"
          title="John Doe"
          nav
        >
          <template v-slot:append>
            <v-btn icon="mdi-arrow-left" @click.stop="rail = !rail"></v-btn>
          </template>
        </v-list-item>

        <v-divider></v-divider>

        <v-list density="compact" nav>
          <v-list-item
            prepend-icon="mdi-tennis"
            title="All courts"
            value="All courts"
          ></v-list-item>
        </v-list>
      </v-navigation-drawer>
    </v-layout>
  </v-card>
</template>
