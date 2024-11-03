<script setup lang="ts">
  import { ref } from "vue";

  const coinRef = ref<HTMLElement>(null);
  const coinSide = ref<boolean>(false);

  function flipCoin() {
    coinSide.value = Math.floor(Math.random() * 2) === 1;
    coinRef.value.textContent = coinSide.value ? "Heads" : "Tails";
  }
</script>

<template>
  <div ref="coinRef" @click="flipCoin" class="coin-flip">C</div>
</template>

<style lang="scss">
  .coin-flip {
    cursor: pointer;
    user-select: none;
    width: 8rem;
    height: 8rem;
    padding: 2rem;
    border-radius: 4rem;
    background-color: #f70;
    font-size: 4rem;
    line-height: 1;
    text-align: center;
  }
</style>
