<template>
  <div class="flex rounded-2xl justify-center items-center shadow-md px-2 py-1 bg-primaryDark text-primary w-auto font-semibold">
    {{ props.text }}
  </div>
</template>
<script setup>
const props = defineProps({
  text: String
})
</script>