<template>
  <div
    class="max-w-sm lg:max-w-[250px] flex flex-col border bg-white overflow-hidden shadow-sm"
  >
    <div class="group overflow-hidden">
      <img
        class="object-cover group-hover:scale-110 aspect-video transition-all ease-out duration-1000"
        :src="imgURL"
        alt=""
      />
    </div>
    <div class="details p-4">
      <h1 class="text-lg font-bold">{{ brand }}</h1>
      <h1 class="text-md font-medium">{{ name }}</h1>
      <!-- <p>{{ desc }}</p> -->
      <div class="flex flex-row justify-between my-2">
        <h1 class="font-bold">${{ price }}</h1>
        <!-- <h1>{{ rating }}⭐</h1> -->
        <div class="flex flex-row items-center">
          <div
            class="text-sm"
            v-for="n in parseInt(rating)"
            :key="n"
          >
            ⭐
          </div>
        </div>
      </div>

      <div class="flex flex-row items-center mt-4">
        <div>sizes: &nbsp;</div>
        <div
          class="flex flex-row flex-wrap"
          v-for="size in sizes"
          v-bind:key="size"
        >
          <p class="bg-black text-white p-2">{{ size }}</p>
          &nbsp;
        </div>
      </div>

      <!-- <div class="inline-block my-2 text-sm p-2 bg-slate-300 text-black">
        #{{ category }}
      </div> -->
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  id: String,
  brand: String,
  name: String,
  desc: String,
  category: String,
  price: Number,
  rating: Number,
  sizes: Array,
  imgURL: String,
});
</script>
