<script setup>
const items = [1,2,3,4,5]
</script>

<template>
  <section class="mx-auto container flex items-center text-center flex-col space-y-2">
        <!-- <div class="p-5 border border-gray-600 w-40" v-for="n in 5"> {{ n }}</div> -->
        <div class="p-5 border border-gray-600 w-40" v-for="item in items"> {{ item }}</div>

    </section>
</template>

<style scoped>

</style>
