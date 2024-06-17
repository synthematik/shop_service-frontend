<template>
  <header class="flex justify-between border-b border-gray-200 px-10 py-10">

    <div class="flex items-center gap-4">
      <img src="/logo.jpg" alt="Logo" class="w-16 rounded-full" />
      <div>
        <h2 class="text-xl font-bold uppercase">Trust Shop</h2>
        <p class="text-slate-400">Лучший магазин на свете</p>
      </div>
    </div>

    <ul class="flex items-center gap-10">
      <li class="flex items-center cursor-pointer gap-3 text-slate-500 hover:text-black">
        <img src="/cart.svg" alt="Cart" />
        <b>1205 руб.</b>
      </li>

      <li class="flex items-center cursor-pointer gap-3 text-slate-500 hover:text-black">
        <img src="/heart.svg" alt="Heart" />
        <b>Закладки</b>
      </li>

      <li class="flex items-center cursor-pointer gap-3 text-slate-500 hover:text-black">
        <img src="/profile.svg" alt="Profile" />
        <b>Профиль</b>
      </li>

    </ul>

  </header>
</template>
