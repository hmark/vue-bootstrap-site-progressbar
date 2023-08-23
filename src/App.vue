<template>
  <SiteProgressBar :active="isLoading" bgClass="bg-danger"></SiteProgressBar>
  <button @click.prevent="isLoading = !isLoading">TOGGLE PROGRESS BAR</button>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import SiteProgressBar from '../lib/SiteProgressBar.vue'
const isLoading = ref(false)
</script>

<style>
@import "bootstrap/scss/bootstrap.scss";
</style>