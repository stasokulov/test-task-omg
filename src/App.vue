<script setup lang="ts">
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <header>
    <div class="wrapper">
      <h1>Тестовое задание для ООО "Омг"</h1>
      <p><a href="https://disk.yandex.ru/edit/d/ucYM3dzDQuoV3bsn9ReKESPegnqahzm72s0qoIz-cKg6NE04WnJrVnZ2QQ" target="_blank">Текст ТЗ</a></p>
      <p><a href="https://syktyvkar.hh.ru/vacancy/98160197" target="_blank">Вакансия</a></p>
    </div>
  </header>

  <main>
    <TheWelcome />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}
</style>
