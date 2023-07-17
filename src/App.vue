<script setup>
const tasks = [
  { id: 1, title: "Complete project proposal", status: "In Progress" },
  { id: 2, title: "Update website content", status: "Completed" },
  { id: 3, title: "Fix bug in user authentication", status: "In Progress" },
  { id: 4, title: "Prepare presentation slides", status: "Pending" },
  { id: 5, title: "Test new feature implementation", status: "Completed" },
];

const person = {
  name: "John Doe",
  age: "45",
  designation: "CTO",
  email: "john@doe.com"
}


</script>

<template>
  <section class="mx-auto container">
    <section class="mx-auto container space-y-3">
      <!-- <div class="p-5 border border-gray-600 text-left" v-for="(task, index) in tasks" :key="index">{{ task.id }} - {{task.title}} </div> -->
      <div class="p-5 border border-gray-600 text-left" v-for="(value, property, index) in person" :key="property">{{ property }} = {{ value }}</div>

    </section>
  </section>
</template>

<style scoped></style>
