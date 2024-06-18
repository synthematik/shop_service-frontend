<script setup>
  import CartItemList from '@/components/CartItemList.vue'
</script>

<template>
  <div class="fixed top-0 left-0 h-full w-full bg-black z-10 opacity-70"></div>
  <div class="bg-white w-96 h-full fixed right-0 top-0 z-20 p-8">
    <div class="flex items-center gap-5 mb-8">
      <svg
        class="opacity-30 cursor-pointer rotate-180 hover:opacity-100 transition hover:-translate-x-1"
        width="16"
        height="16"
        viewBox="0 0 16 16"
        fill="none"
        xmlns="http://www.w3.org/2000/svg">

        <path d="M1 7H14.7143" stroke="black" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
        <path d="M8.71436 1L14.7144 7L8.71436 13" stroke="black" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>

      <h2 class="text-2xl font-bold">Корзина</h2>
    </div>
    <CartItemList />

    <div class="flex flex-col gap-4 mt-7">

      <div class="flex gap-2">
        <span>Скидка:</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b>500 руб</b>
      </div>

      <div class="flex gap-2">
        <span>Итого:</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b>12900 руб</b>
      </div>

      <button
        disabled=""
        class="mt-4 bg-green-500 w-full rounded-xl py-3 text-white transition hover:bg-green-600 active:bg-green-700 disabled:bg-slate-400 cursor-pointer"
      >Оформить заказ
      </button>

    </div>



  </div>
</template>
