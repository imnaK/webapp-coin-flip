<script setup lang="ts">
  import CoinFlip from "@/components/CoinFlip.vue";
</script>

<template>
  <div>
    <a href="https://security.tyrem-envalura.de" target="_blank">
      <img src="/logo.svg" class="logo" alt="Tyrem Envalura Logo" />
    </a>
  </div>
  <CoinFlip />
</template>

<style scoped>
  .logo {
    height: 8rem;
    padding: 2rem;
    will-change: filter;
    transition: filter 0.3s;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #ff07);
  }
</style>
