<template>
  <!-- <NuxtLink :to="`/products/${p.id}`">{{ p.title }}</NuxtLink> -->
  <div class="card text-center">
    <img :src="product.image" :alt="product.title" class="thumb" />
    <p class="font-bold text-gray-500 m-4 truncate">{{ product.title }}</p>
    <NuxtLink :to="`/products/${product.id}`">
      <p class="btn my-4">View Details</p>
    </NuxtLink>
  </div>
</template>

<script setup>
const { product } = defineProps(["product"]);
</script>
<style scoped>
.thumb {
    @apply max-h-32 max-w-[70%] my-0 mx-auto
}
</style>
