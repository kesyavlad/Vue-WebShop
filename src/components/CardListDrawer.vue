<script setup>
import CardDrawer from './CardDrawer.vue'

const onClickDelete = () => {
  alert('delete')
}
</script>

<template>
  <CardDrawer
    imageURL="/sneakers/sneakers-1.jpg"
    title="Nike Best V111 for Men"
    :onClickDelete="onClickDelete"
  />
  <CardDrawer
    imageURL="/sneakers/sneakers-2.jpg"
    title="Nike Best V33 for Men"
    :onClickDelete="onClickDelete"
  />
  <CardDrawer
    imageURL="/sneakers/sneakers-3.jpg"
    title="Nike Best V22 for Men"
    :onClickDelete="onClickDelete"
  />
</template>
