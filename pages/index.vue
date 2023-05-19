<template>
  <!-- <Hero class="h-screen" /> -->

  <div
    class="h-screen p-16 pt-48 lg:pt-64 lg:p-32 bg-[url('~/assets/hero2.jpg')] bg-cover"
  >
    <h1 class="lg:w-2/3 text-4xl font-bold mb-8">
      Unleash Your Inner Fashionista with Our Collection
    </h1>
    <p class="lg:w-3/6 text-lg font-semibold leading-relaxe overflow-hidden">
      Our collection helps you discover your sense of style and express it
      confidently through fashion, unleashing your inner fashionista.
    </p>
  </div>
  <div class="h-full p-16 md:p-32">
    <h1 class="text-2xl font-bold mb-8">Dashboard</h1>
    <p class="leading-relaxe overflow-hidden">
      Lorem ipsum dolor, sit amet consectetur adipisicing elit. Impedit,
      nesciunt saepe cum sint maxime amet vel necessitatibus aliquam numquam a,
      magnam et id quidem porro quas recusandae omnis veniam. Dolor dolorum
      assumenda temporibus delectus voluptatum officia debitis obcaecati id
      magni corrupti provident ad, totam ducimus? Quidem, neque id vitae ipsam
      corporis, eveniet quasi eligendi cumque, labore ex ipsa fugit sapiente
      distinctio sequi laborum animi inventore alias? Facilis molestiae,
      dignissimos explicabo eos beatae magni aut labore perspiciatis blanditiis,
      reprehenderit eum id pariatur velit. Nobis aperiam vel numquam quaerat
      obcaecati vero odio aut voluptatum facere, itaque omnis nihil sed error
      quam consequuntur quisquam placeat molestiae! Voluptates ratione ad magni
      sapiente labore placeat vitae cum, dicta obcaecati nemo qui architecto!
      Molestiae placeat earum doloremque labore expedita perferendis possimus,
      ut est vel, eveniet atque reprehenderit, beatae sunt ratione veniam autem
      nesciunt. Eveniet voluptatum ipsam facere quisquam sit tempore optio,
      molestias nulla aliquid laboriosam ex.
    </p>
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
