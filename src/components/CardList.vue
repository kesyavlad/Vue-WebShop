<script setup>
import CardProduct from './CardProduct.vue'

const onClickAdd = () => {
  alert('add')
}
const onChangeLike = () => {
  alert('change')
}
</script>
<template>
  <CardProduct
    title="TestText"
    :price="5000"
    imageURL="/sneakers/sneakers-1.jpg"
    :is-added="isAdded"
    :is-favorite="isFavorite"
    :onClickAdd="onClickAdd"
    :onChangeLike="onChangeLike"
  />
  <CardProduct
    title="TestText"
    :price="5000"
    imageURL="/sneakers/sneakers-1.jpg"
    :is-added="isAdded"
    :is-favorite="isFavorite"
    :onClickAdd="onClickAdd"
    :onChangeLike="onChangeLike"
  />
</template>
