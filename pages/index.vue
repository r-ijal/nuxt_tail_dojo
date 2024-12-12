<template>
  <section class="flex flex-col justify-center items-center gap-4 h-fit">
    <h1 class="text-3xl font-bold underline text-cyan-500">Hello world!</h1>

    <h1>Demo with auto imports</h1>
    <form class="flex gap-2" @submit.prevent="hello">
      <CustomInput v-model="message" />
      <button
        class="text-base px-4 py-2 text-emerald-500 hover:bg-emerald-400 hover:text-white rounded-lg border"
        type="submit"
      >
        Hello
      </button>
    </form>
  </section>
</template>

<script setup>
const message = ref("Nuxt");

function hello() {
  sayHello(message.value);
}
</script>
