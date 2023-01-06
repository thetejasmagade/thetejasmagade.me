<script lang="ts" setup>
</script>

<template>
  <header>
    <div class="flex justify-between items-center max-w-8xl mx-auto mx-auto px-8 sm:py-4 sm:px-40 py-3">
        <img src="~/assets/signature.svg" height="50px" width="50px">
    </div>
  </header>
</template>

<style>
header {
  border-style: none;
  backdrop-filter: blur(10px);
  position: sticky;
  top: 0;
  width: 100%;
  z-index: 50;
}

nav .icon {
  width: 1rem;
  height: 1rem;
}

@media (max-width: 768px) {
  nav .icon {
    display: none !important;
  }
}
</style>