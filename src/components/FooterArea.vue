<script setup>
import { ref, onMounted } from 'vue'
const year = ref('')

const getYear = () => {
  const now = new Date()
  year.value = now.getFullYear()
}

onMounted(() => {
  getYear()
})
</script>
<template>
  <footer class="bg-black h-10 flex items-center justify-center">
    <p class="text-white">Copyright © {{ year }} ChunMing - All right reserved</p>
  </footer>
</template>
