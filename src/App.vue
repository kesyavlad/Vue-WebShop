<script setup>
import HeaderPage from './components/headerPage.vue'
import CardList from './components/CardList.vue'
</script>

<template>
  <div
    class="w-4/5 m-auto bg-white rounded-xl shadow-xl my-10"
  >
    <HeaderPage />
    <div class="p-10">
      <h2 class="text-3xl font-bold">All Sneakers</h2>
      <div
        class="grid grid-cols-1 gap-5 mt-7 sm:grid-cols-2 lg:grid-cols-4"
      >
        <CardList />
      </div>
    </div>
  </div>
</template>

<style></style>
