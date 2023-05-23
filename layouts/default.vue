<template>
  <div>
    <Navbar />
    <main>
      <slot />
    </main>
    <Footer />
  </div>
</template>

<style>
/* width */
::-webkit-scrollbar {
  width: 10px;
}

::-webkit-scrollbar-track {
  /* background: transparent; */
  display: none;
}

/* ::-webkit-scrollbar-thumb {
  background-clip: padding-box;
  border-radius: 0;
  background-color: #000;
} */

::-webkit-scrollbar-thumb {
  border-right: 10px solid black;
}
</style>
