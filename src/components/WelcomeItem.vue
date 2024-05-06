<script setup lang="ts">

const list: number[] = new Array(12).fill('').map(() => Math.round(Math.random()*10))
</script>

<template>
  <div class="item">
    <h3><slot></slot></h3>
    <div class="details">
      <div v-for="item in list" :key="item" class="cell-wrapper">
        <div class="cell">{{ item }}</div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.item {
  margin-top: 2rem;
  display: flex;
  align-items: center;
  column-gap: 10px;
}

.details {
  display: flex;
  column-gap: 10px;
  padding: 10px;
  overflow-y: auto;
  border: 1px solid var(--color-border);
  border-radius: var(--border-radius);
  box-shadow: var(--box-shadow);
}

.cell-wrapper {
  &:hover {
    .cell {
      transform: scale(80%);
    }
  }
}

.cell {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 40px;
  min-width: 40px;
  height: 40px; 
  border: 1px solid var(--color-border);
  border-radius: var(--border-radius);
  box-shadow: var(--box-shadow);
  transition: transform 1s;
}

h3 {
  font-size: 1.2rem;
  font-weight: 500;
  margin-bottom: 0.4rem;
}
</style>
