<template>
  <footer
    class="pt-16 px-32 flex flex-col justify-center bg-black text-white gap-8 border-t border-black"
  >
    <div class="w-full flex flex-row flex-wrap justify-between items-start">
      <div class="basis-1/4 brand">
        <p class="text-2xl font-bold">StyleHub.</p>
        <p class="text-md font-light mt-4">
          "Discover the Latest Fashion Must-Haves Here"
        </p>
      </div>
      <ul class="basis-1/3 text-right flex flex-col gap-8 text-lg">
        <li><nuxt-link to="/">Home</nuxt-link></li>
        <li><nuxt-link to="/products">products</nuxt-link></li>
        <li><nuxt-link to="/category">Category</nuxt-link></li>
        <li><nuxt-link to="/account">Account</nuxt-link></li>
      </ul>
      <ul class="flex-auto text-right flex flex-col gap-8 text-lg">
        <li><nuxt-link to="#">Jacket</nuxt-link></li>
        <li><nuxt-link to="#">Shirt</nuxt-link></li>
        <li><nuxt-link to="#">Jeans</nuxt-link></li>
        <li><nuxt-link to="#">Hats</nuxt-link></li>
      </ul>
    </div>
    <div class="text-center my-8 pt-8 border-white border-t">
      Made ugal-ugalan 💥 by Akbar
    </div>
  </footer>
</template>
