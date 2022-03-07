<template>
  <h2>{{ title }}</h2>
</template>

<script lang="ts" setup>
import { ref } from 'vue';

defineProps<{ title: string }>();
</script>
