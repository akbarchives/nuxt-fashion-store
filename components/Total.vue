<template>
  <div class="flex justify-center">
    <div class="px-16 py-8 max-w-md bg-amber-300">
      <h1 class="font-bold my-4 border-b border-black">Total Harga</h1>
      <label
        class="my-2"
        for="total"
        >Masukkan Total Harga Pembelian:</label
      >
      <input
        class="my-2 p-2 w-full"
        type="number"
        id="total"
        placeholder="Contoh: 80000"
      />

      <button
        class="px-4 py-2 bg-black text-white hover:bg-gray-900"
        onclick="calculateDiscount()"
      >
        Hitung Diskon
      </button>

      <div id="result">
        <div class="mt-4 flex justify-between">
          <p>Harga</p>
          <p
            class="font-bold"
            id="amount"
          >
            Rp.0
          </p>
        </div>
        <div class="flex justify-between border-b border-black">
          <p>Diskon</p>
          <p
            class="font-bold"
            id="discountAmount"
          >
            Rp.0
          </p>
        </div>
      </div>
      <div class="flex justify-between w-full font-bold my-4">
        <p>Total Bayar</p>
        <p id="totalAfterDiscount">Rp.0</p>
      </div>
    </div>
  </div>
</template>

<script>
function calculateDiscount() {
  const totalInput = document.getElementById('total');
  const total = parseFloat(totalInput.value);

  let discountAmount = 0;
  let totalAfterDiscount = 0;

  if (total >= 100000) {
    discountAmount = total * 0.1;
  } else if (total >= 50000) {
    discountAmount = total * 0.05;
  }

  totalAfterDiscount = total - discountAmount;

  const amountDisplay = document.getElementById('amount');
  const discountAmountDisplay = document.getElementById('discountAmount');
  const totalAfterDiscountDisplay =
    document.getElementById('totalAfterDiscount');

  amountDisplay.textContent = `Rp.${total}`;
  discountAmountDisplay.textContent = `R.${discountAmount}`;
  totalAfterDiscountDisplay.textContent = `Rp.${totalAfterDiscount}`;
}
</script>
