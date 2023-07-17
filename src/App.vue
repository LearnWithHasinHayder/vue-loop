<script setup>
const persons = [
  {
    id: 1,
    name: "Jane Doe",
    profilePhoto: "//tailus.io/sources/blocks/classic/preview/images/woman1.jpg",
    jobTitle: "CEO, Co-Founder",
  },
  {
    id: 2,
    name: "John Doe",
    profilePhoto: "//tailus.io/sources/blocks/classic/preview/images/man.jpg",
    jobTitle: "CTO",
  },
  {
    id: 3,
    name: "Jessy Doe",
    profilePhoto: "//tailus.io/sources/blocks/classic/preview/images/woman.jpg",
    jobTitle: "COO",
  }
];
</script>

<template>
  <section class="mx-auto container">
    <div class="py-20 bg-gray-50">
        <div class="container mx-auto px-6 px-32">
            <div class="mb-16 text-center">
                <h2 class="mb-4 text-center text-2xl text-gray-900 font-bold text-4xl">Team Member</h2>
                <p class="text-gray-600 w-8/12 mx-auto">Lorem ipsum dolor sit amet consectetur adipisicing elit. Magni deleniti veniam laudantium itaque perferendis dolor maxime incidunt voluptatem. </p>
            </div>
            <div class="grid gap-12 items-center grid-cols-3">
                <div class="space-y-4 text-center" v-for="(person, index) in persons" :key="person.id">
                    <img class="w-64 h-64 mx-auto object-cover rounded-xl w-64" :class="2==person.id?'h-80':'h-60'" :src="person.profilePhoto">
                    <!-- <img class="w-64 h-64 mx-auto object-cover rounded-xl w-64" :class="1==index?'h-80':'h-60'" :src="person.profilePhoto"> -->
                    <div>
                        <h4 class="text-2xl">{{ person.name }}</h4>
                        <span class="block text-sm text-gray-500">{{ person.jobTitle }}</span>
                    </div>
                </div>
                
            </div>
        </div>
    </div>
  </section>
</template>

<style scoped></style>
