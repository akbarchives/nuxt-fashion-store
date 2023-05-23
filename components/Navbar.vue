<template>
  <nav
    class="flex flex-row justify-between items-center px-4 py-8 md:px-16 md:py-8 border-b border-black fixed w-full bg-white text-primary"
  >
    <div class="brand">
      <p class="text-3xl font-bold text-black">
        Style<span class="text-white bg-black">Hub</span>
      </p>
    </div>
    <ul class="flex flex-row gap-2 text-lg font-medium">
      <li>
        <nuxt-link
          class="px-2 md:px-6 py-3 hover:bg-black hover:text-white"
          to="/"
          >Home</nuxt-link
        >
      </li>
      <li>
        <nuxt-link
          class="px-2 md:px-6 py-3 hover:bg-black hover:text-white"
          to="/products"
          >Products</nuxt-link
        >
      </li>
      <!-- <li>
        <nuxt-link
          class="px-2 md:px-6 py-3 hover:bg-black hover:text-white"
          to="/category"
          >Category</nuxt-link
        >
      </li>
      <li>
        <nuxt-link
          class="px-2 md:px-6 py-3 hover:bg-black hover:text-white"
          to="/account"
          >Account</nuxt-link
        >
      </li> -->
    </ul>
  </nav>
</template>

<style scoped>
nav {
  z-index: 101;
}
.router-link-active {
  @apply bg-black text-white;
}
</style>
