<template>
  <SiteProgressBar :active="isLoading" bgClass="bg-primary"></SiteProgressBar>
  <button v-if="!isLoading" @click.prevent="isLoading = true">START</button>
  <button v-if="isLoading" @click.prevent="isLoading = false">STOP</button>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import SiteProgressBar from '../lib/SiteProgressBar.vue'

const isLoading = ref(false)
</script>

<style>
@import "bootstrap/scss/bootstrap.scss";
</style>