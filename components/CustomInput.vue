<script setup>
defineProps(["modelValue"]);
defineEmits(["update:modelValue"]);
</script>

<template>
  <input
    class="border rounded-lg"
    :value="modelValue"
    @input="$emit('update:modelValue', $event.target.value)"
  />
</template>
