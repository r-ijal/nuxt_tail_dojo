<template>
  <div>
    <h1>About page</h1>

    <div>
      <pre>
        {{ data }}
      </pre>
    </div>
  </div>
</template>

<script setup>
// const { data } = await useFetch('/api/ninja?name=mario', {
//   method: 'post',
//   body: { age: 30 }
// })

// const { data } = await useFetch("/api/ninja");
const { data } = await useFetch("/api/currency/IDR");
</script>
<style scoped></style>
