
<template>
  <div class="rounded-md shadow-md px-2 py-1 text-primary w-full font-bold">
    {{ props.text }}
  </div>
</template>
<script setup>
const props = defineProps({
  type: {
    type: String,
    default: "primary"
  },
  text: String
})
</script>