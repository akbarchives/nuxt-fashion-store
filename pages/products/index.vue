<template>
  <div class="w-full p-16 sm:px-32 pt-48 md:pt-48">
    <h1 class="text-2xl font-bold mb-8">Collections</h1>
    <div
      class="collections gap-2 flex flex-row flex-wrap justify-center md:justify-normal"
    >
      <NuxtLink
        class=""
        v-for="product in products"
        :to="`/products/${product.id}`"
        :key="product.id"
      >
        <Card
          class="flex flex-row"
          :brand="product.brand"
          :name="product.name"
          :desc="product.description"
          :category="product.category"
          :price="product.price"
          :rating="product.rating"
          :imgURL="product.image"
          :sizes="product.sizes"
        />
      </NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: [
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
      ],
    };
  },
};
</script>
