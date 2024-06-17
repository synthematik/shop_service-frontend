<script setup>
defineProps({
  imageUrl: String,
  title: String,
  price: Number,
  isFavorite: Boolean,
  isAdded: Boolean,
  onclickAdd: Function,
  onclickFavorite: Function,
})
</script>

<template>
  <div>
    <div class="relative border border-slate-100 rounded-3xl p-8 cursor-pointer transition hover:-translate-y-2 hover:shadow-xl">

      <img
        :src="isFavorite ? '/like-2.svg' : '/like-1.svg'"
        alt="Like 2"
        class="absolute top-8 left-8"
        @click="isFavorite"
      />

      <img :src="imageUrl" alt="Sneakers 1"  />

      <p class="mt-2">{{ title }}</p>

      <div class="flex justify-between mt-5">

        <div class="flex flex-col text-lg">
          <span class="text-slate-400">Цена: </span>
          <b >{{ price }} руб</b>
        </div>

        <img
          :src="!isAdded ? '/plus.svg' : '/checked.svg'"
          alt="Plus"
          @click="isAdded"
        />

      </div>
    </div>
  </div>
</template>
