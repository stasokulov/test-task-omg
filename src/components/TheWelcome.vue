<script setup lang="ts">
import WelcomeItem from './WelcomeItem.vue'

const list: number[] = [...new Array(101).keys()]
</script>

<template>
  <WelcomeItem v-for="item in list" :key="item">{{ item }}</WelcomeItem>
</template>
