

<template>
  <Header />
  <div class="container-cards">

    <Card />
    <Card />
    <Card />
    <Card />
  </div>
  <button @click="warn()">click</button>
</template>

<script setup lang="ts">
import Header from './components/Header.vue';
import Card from './components/Card.vue';

function warn() {
  alert("Olá, mundo!")
}
</script>

<style scoped>
.container-cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  gap: 20px;
  padding: 40px;
}
</style>
