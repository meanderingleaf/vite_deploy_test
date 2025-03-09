<script setup>
import HelloWorld from './components/HelloWorld.vue'
import Button from "primevue/button"
import Card from "primevue/card"

const images = ["img/vue.svg", "img/absart.jpg"]

</script>

<template>

  <Card v-for="image in images" :key="image">

    <template #content>
      <img :src="image" />
    </template>
  </Card>
  
</template>