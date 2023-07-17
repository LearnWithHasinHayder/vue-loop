<script setup>
const tasks = [
  "Complete project proposal",
  "Update website content",
  "Fix bug in user authentication",
  "Prepare presentation slides",
  "Test new feature implementation",
];
</script>

<template>
  <section class="mx-auto container">
    <section class="mx-auto container space-y-3">
        <div class="p-5 border border-gray-600 text-left" v-for="(task, index) in tasks">{{ index+1 }}. {{task}}</div>
    </section>
  </section>
</template>

<style scoped>

</style>
