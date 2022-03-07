<template>
  <button @click="toggle = !toggle">Toggle</button>
  <template v-if="toggle">
    <Blog v-for="title of titles" :title="title" :key="title" class="parent"
  /></template>
</template>

<script setup lang="ts">
import { onMounted, reactive, ref } from 'vue';
import Blog from './Blog.vue';

const titles = ref(['Un titre', 'Un autre titre', 'Encore un dernier titre']);

const toggle = ref(true);
</script>

<style scoped lang="scss"></style>
