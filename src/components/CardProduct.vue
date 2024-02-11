<script setup>
defineProps({
  imageURL: String,
  title: String,
  price: Number,
  isFavorite: Boolean,
  isAdded: Boolean,
  onClickAdd: Function,
  onChangeLike: Function
})
</script>

<template>
  <div
    class="relative bg-white border border-slate-200 shadow-md rounded-xl p-8 cursor-pointer transition hover:shadow-2xl hover:-translate-y-2"
  >
    <img
      @click="onChangeLike"
      :src="!isFavorite ? '/like-1.svg' : '/like-2.svg'"
      alt="like"
      class="absolute top-2 left-2"
    />
    <img :src="imageURL" alt="sneakers1" />
    <p class="my-5">{{ title }}</p>
    <div class="flex justify-between">
      <div class="flex flex-col">
        <span class="text-slate-400">Price:</span>
        <b>{{ price }}$</b>
      </div>
      <img
        @click="onClickAdd"
        :src="!isAdded ? '/plus.svg' : '/checked.svg'"
        alt="plus"
      />
    </div>
  </div>
</template>
