<template>
  <div class="hero p-32 pt-48 bg-[url('~/assets/hero2.jpg')] bg-cover">
    <h1
      class="w-1/2 leading-tight text-4xl text-primary drop-shadow-2xl font-bold mb-8"
    >
      Unleash Your Inner Fashionista with Our Collection
    </h1>
    <p
      class="w-1/2 text-md text-zinc-800 italic font-semibold drop-shadow-2xl leading-relaxe overflow-hidden"
    >
      Lorem ipsum dolor, sit amet consectetur adipisicing elit. Saepe vel magnam
      non nostrum numquam odio ex ad. Excepturi molestias inventore ducimus, eos
      id officiis pariatur?
    </p>
    <div class="box flex justify-center">
      <div class="w-full p-16 bg-white rounded-[50px] shadow-xl border">
        <h1 class="text-3xl font-bold mb-12">New Collection</h1>
        <div class="collection flex flex-row gap-4 justify-between">
          <Card />
          <Card />
          <Card />
          <Card />
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.box {
  position: relative;
  top: 100px;
  z-index: 100;
}
</style>
