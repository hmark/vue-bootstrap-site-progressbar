# Vue Bootstrap Site ProgressBar

> Simple site progressbar for Vue3 & Bootstrap5 project

## Installation

```bash
npm install vue-bootstrap-site-progressbar
```

## Usage with Composition API

```vue
<template>
  <SiteProgressBar :active="isLoading" bgClass="bg-primary"></SiteProgressBar>
  <button v-if="!isLoading" @click.prevent="isLoading = true">START</button>
  <button v-if="isLoading" @click.prevent="isLoading = false">STOP</button>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import { SiteProgressBar } from 'vue-bootstrap-site-progressbar'

const isLoading = ref(false)
</script>

<style>
@import 'bootstrap/scss/bootstrap.scss';
</style>
```
