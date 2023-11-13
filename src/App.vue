<script setup lang="ts">
import AppHeader from './components/common/AppHeader.vue'
import AppFooter from './components/common/AppFooter.vue'
</script>

<template>
  <q-layout view="lHh lpr lFf" container style="height: 100vh" class="shadow-2 rounded-borders">
    <AppHeader/>
    <AppFooter/>
    <RouterView />
  </q-layout>
</template>
