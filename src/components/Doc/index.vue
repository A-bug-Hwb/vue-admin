<template>
  <div>
    <svg-icon icon-class="question" @click="goto" />
  </div>
</template>

<script setup>
const url = ref(import.meta.env.VITE_APP_BASE_API + "doc.html");

function goto() {
  window.open(url.value)
}
</script>