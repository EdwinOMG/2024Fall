<script setup lang="ts"></script>

<template>
  <div class="flyout"></div>
</template>

<style scoped>
.flyout {
  position: fixed;
  top: 56px;
  right: 0;
  bottom: 0;
  width: 20rem;
  background-color: #fff;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.8);
  z-index: 1000;
  transform: translateX(100%);
}
.flyout.hover,
.flyout.isOpen {
  transform: translateX(0);
}
</style>
