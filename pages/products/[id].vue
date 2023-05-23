<script setup>
const route = useRoute();
const products = [
  {
    id: 1,
    name: 'Classic Stripes Shirt',
    brand: 'Example Brand',
    category: 'T-Shirts',
    price: 19.99,
    color: 'Black',
    rating: 5,
    sizes: ['S', 'M', 'L'],
    description:
      'A classic stripes shirt made from soft and comfortable fabric.',
    image:
      'https://images.unsplash.com/photo-1586798658502-0dc367cb2776?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=600&ixid=MnwxfDB8MXxyYW5kb218MHx8c2hpcnR8fHx8fHwxNjg0NTAxOTM1&ixlib=rb-4.0.3&q=80&utm_campaign=api-credit&utm_medium=referral&utm_source=unsplash_source&w=800',
  },
  {
    id: 2,
    name: 'Slim Fit Jeans',
    brand: 'Denim Co.',
    category: 'Jeans',
    price: 49.99,
    color: 'Blue',
    rating: 5,
    sizes: ['28', '30', '32', '34'],
    description: 'Stylish slim fit jeans in a trendy blue color.',
    image:
      'https://images.unsplash.com/photo-1546635834-78554e816d55?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=600&ixid=MnwxfDB8MXxyYW5kb218MHx8amVhbnN8fHx8fHwxNjg0NTAyMDkx&ixlib=rb-4.0.3&q=80&utm_campaign=api-credit&utm_medium=referral&utm_source=unsplash_source&w=800',
  },
  {
    id: 3,
    name: 'Leather Jacket',
    brand: 'Fashion Forward',
    category: 'Jackets',
    price: 129.99,
    color: 'Brown',
    rating: 4,
    sizes: ['S', 'M', 'L', 'XL'],
    description: 'A high-quality leather jacket with a stylish design.',
    image:
      'https://images.unsplash.com/photo-1520975916090-3105956dac38?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=600&ixid=MnwxfDB8MXxyYW5kb218MHx8bGVhdGhlcmphY2tldHx8fHx8fDE2ODQ1MDIxNTc&ixlib=rb-4.0.3&q=80&utm_campaign=api-credit&utm_medium=referral&utm_source=unsplash_source&w=800',
  },
  {
    id: 4,
    name: 'Casual White T-Shirt',
    brand: 'Fan Tee',
    category: 'Shirt',
    price: 129.99,
    color: 'Brown',
    rating: 4,
    sizes: ['S', 'M', 'L', 'XL'],
    description: 'A comfort T-shirt with no design.',
    image:
      'https://images.unsplash.com/photo-1622445275463-afa2ab738c34?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=600&ixid=MnwxfDB8MXxyYW5kb218MHx8aGF0fHx8fHx8MTY4NDUwMjE5Mg&ixlib=rb-4.0.3&q=80&utm_campaign=api-credit&utm_medium=referral&utm_source=unsplash_source&w=800',
  },
  {
    id: 5,
    name: 'Black Hat',
    brand: 'Black Jack',
    category: 'Hats',
    price: 129.99,
    color: 'Brown',
    rating: 5,
    sizes: ['All Size'],
    description: 'A high-quality Hat with best materials.',
    image:
      'https://images.unsplash.com/photo-1606483956061-46a898dce538?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=600&ixid=MnwxfDB8MXxyYW5kb218MHx8aGF0fHx8fHx8MTY4NDUwMjM2Mw&ixlib=rb-4.0.3&q=80&utm_campaign=api-credit&utm_medium=referral&utm_source=unsplash_source&w=800',
  },
];

const id = route.params.id;
const product = products[id - 1];
</script>

<template>
  <div
    class="p-8 md:p-16 pt-48 md:pt-48 flex flex-row flex-wrap md:flex-nowrap md:object-cover"
  >
    <div
      class="group basis-full md:basis-1/2 lg:basis-1/3 overflow-hidden bg-white object-cover"
    >
      <img
        class="group hover:scale-125 transition-all ease duration-500 lg:aspect-square object-cover"
        :src="product.image"
        alt=""
      />
    </div>
    <div
      class="basis-full md:basis-1/2 lg:basis-2/3 border md:border-0 border-black p-8 flex flex-col justify-between"
    >
      <div class="mb-8 md:mb-0">
        <h1 class="text-xl font-bold">{{ product.brand }}</h1>
        <h1 class="text-lg font-medium">
          {{ product.name }} |
          <span
            class="text-lg"
            v-for="n in parseInt(product.rating)"
            :key="n"
          >
            ⭐
          </span>
        </h1>
        <h1 class="text-xl font-bold">$ {{ product.price }}</h1>
      </div>
      <div class="mb-8 lg:mb-0">
        <h2 class="text-lg font-medium">Description :</h2>
        <h2 class="text-md">{{ product.description }}</h2>
        <div class="flex flex-row items-center mt-4">
          <div>sizes: &nbsp;</div>
          <div
            class="flex flex-row flex-wrap"
            v-for="size in product.sizes"
            v-bind:key="size"
          >
            <p class="bg-black hover:bg-zinc-800 text-white p-2">{{ size }}</p>
            &nbsp;
          </div>
        </div>
      </div>
      <div class="flex flex-row justify-between items-center mt-4">
        <div class="py-2 px-4 bg-slate-300 hover:bg-slate-400 text-black">
          #{{ product.category }}
        </div>
        <button class="py-2 px-4 bg-red-500 hover:bg-red-600 text-white">
          Add to Cart
        </button>
      </div>
    </div>
  </div>
</template>
