<script setup lang="ts">
import { ref } from 'vue'

const search = ref('')
</script>

<template>
  <q-page-container>
    <q-page class="q-pa-md fixed-center" style="min-height: 0;">
      <h1 class="text-h4">入力してください</h1>
      <div class="q-pa-md" style="max-width: 350px">
        <div class="q-gutter-md">
          <q-input
            v-model="search"
            debounce="50"
            filled
            placeholder="Search"
          >
            <template v-slot:append>
              <q-icon name="search" />
            </template>
          </q-input>
        </div>
      </div>
    </q-page>
  </q-page-container>
</template>
