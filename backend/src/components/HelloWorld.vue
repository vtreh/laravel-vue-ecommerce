<script setup>
import { ref, computed } from 'vue'
import store from '../store';

defineProps({
  msg: String,
})

const test = computed(() => store.state.test);
const count = ref(0)
</script>

<template>
  <h1 class="bg-purple-500">{{ test }}</h1>
</template>

<style scoped>

</style>
