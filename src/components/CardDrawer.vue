<script setup>
defineProps({
  imageURL: String,
  title: String,
  price: Number,
  onClickDelete: Function
})
</script>

<template>
  <div
    class="flex gap-2 items-center bg-white border border-slate-200 shadow-md rounded-xl p-3 my-4"
  >
    <img :src="imageURL" alt="sneakers" class="w-20 h-16" />
    <div class="flex items-start gap-4">
      <div class="flex flex-col gap-2">
        <p style="overflow-wrap: anywhere">{{ title }}</p>
        <b>{{ price }}</b>
      </div>
      <img
        src="/close.svg"
        alt="delete"
        class="opacity-40 hover:opacity-100 transition cursor-pointer"
        @click="onClickDelete"
      />
    </div>
  </div>
</template>
