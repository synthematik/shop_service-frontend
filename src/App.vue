<script setup>
  import Header from '@/components/Header.vue'
  import CardList from '@/components/CardList.vue'
</script>

<template>
  <div class="bg-white w-11/12 m-auto rounded-2xl shadow-xl mt-10 mb-10">
    <Header />

    <div class="p-10">
      <h2 class="text-3xl font-bold mb-8">Все кроссовки</h2>

      <CardList />
    </div>



  </div>
</template>
