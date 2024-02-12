<script setup>
import CardListDrawer from './CardListDrawer.vue'
const onClickBack = () => {
  alert('back')
}
</script>

<template>
  <div class="fixed top-0 left-0 h-full w-full bg-black z-10 opacity-70"></div>
  <div class="bg-white w-96 overflow-auto h-full fixed right-0 top-0 z-20 p-8">
    <div class="flex item-baseline align-center gap-3">
      <img
        src="/back.svg"
        alt="back"
        class="w-25 h-25 my-auto cursor-pointer opacity-25 hover:opacity-100 transition hover:-translate-x-1"
        @click="onClickBack"
      />
      <h2>Корзина</h2>
    </div>
    <div class="flex flex-col justify-between h-full">
      <div>
        <CardListDrawer />
      </div>
      <div>
        <div class="flex flex-col gap-4">
          <div class="flex gap-2">
            <span>Result</span>
            <div class="flex-1 border-b border-dashed"></div>
            <b>600$</b>
          </div>
          <div class="flex gap-2">
            <span>Nalog 10%</span>
            <div class="flex-1 border-b border-dashed"></div>
            <b>60$</b>
          </div>
        </div>
        <button class="bg-lime-500 w-full rounded-xl py-3 text-white my-4">
          Order
        </button>
      </div>
    </div>
  </div>
</template>
