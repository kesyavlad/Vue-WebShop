<template>
  <header
    class="flex justify-between border-b border-slate-300 px-8 py-5"
  >
    <div class="flex items-center gap-4">
      <img src="/logo.png" alt="Logo" class="w-10" />
      <div>
        <h2 class="text-xl font-bold uppercase">
          Vue Sneakers
        </h2>
        <p class="text-slate-400 text-xs">
          Best Shop Sneakers
        </p>
      </div>
    </div>
    <ul class="flex gap-4">
      <li
        class="flex items-center cursor-pointer text-gray-500 hover:text-black"
      >
        <img src="/cart.svg" alt="cart" class="size-4" />
        <b class="pl-1">200$</b>
      </li>
      <li
        class="flex items-center cursor-pointer text-gray-500 hover:text-black"
      >
        <img src="/heart.svg" alt="like" class="size-4" />
        <span class="pl-1">Save</span>
      </li>
      <li
        class="flex items-center cursor-pointer text-gray-500 hover:text-black"
      >
        <img
          src="/profile.svg"
          alt="profile"
          class="size-4"
        />
        <span class="pl-1">Profile</span>
      </li>
    </ul>
  </header>
</template>
