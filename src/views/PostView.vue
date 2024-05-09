<template>
  <h1>Sección Posts</h1>
  <p>{{ postId }}</p>
</template>

<script setup>
import { onMounted, ref } from "vue";
import { useRoute } from "vue-router";

let postId = ref();

onMounted(() => {
  const route = useRoute();
  postId.value = route.params.id;
});
</script>
