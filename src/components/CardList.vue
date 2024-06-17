<script setup>
import Card from '@/components/Card.vue'
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <Card
      image-url="/sneakers/sneakers-1.jpg"
      title="Sneaker Sneakers"
      :price="1000"
      :is-favorite="true"
      :is-added="true"
    />
  </div>
</template>
