<script setup lang="ts">
import Header from './components/Header.vue'
import Background from './components/Background.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <div class="app">
    <Header />

    <main class="content">
      <Background />
    </main>

    <Footer />
  </div>
</template>

<style>
  .app {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
  }
  .content {
  flex: 1;
  }
  body{
      margin: 0;
      height: 100%;
      padding:0%;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
  }
</style>
