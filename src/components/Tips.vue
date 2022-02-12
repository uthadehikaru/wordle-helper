<template>
  <div
    class="bg-white text-black fixed max-w-lg h-full w-full top-0 z-20 px-4 sm:px-6 overflow-y-scroll"
  >
    <header class="relative mb-2">
      <h1 class="text-base font-bold my-2">PETUNJUK PENGGUNAAN</h1>
      <v-icon
        name="md-close"
        scale="1.2"
        class="absolute right-0 top-0 text-gray-500 cursor-pointer"
        @click="$emit('close')"
      />
    </header>

    <div class="text-left text-sm border-b border-gray-300 py-3">
      <p>
        1. Mulai permainan
        <a
          class="hyperlink"
          href="https://katla.vercel.app/"
          target="_blank"
          >Katla</a
        >
      </p>
      <p>2. Tebak sebuah kata dan dapatkan petunjuk jawaban (hijau, kuning, atau abu-abu)</p>
      <p>
        3. Masukkan tebakan kamu disini dan <b>klik tiap huruf</b> untuk mengubah petunjuk jawaban lalu tekan enter
      </p>
      <p>
        4. Semua kata yang terkait dengan petunjuk jawaban kamu akan muncul di bagian kanan →
      </p>
      <p>5. Pilih satu kata, lalu kembali ke no 2</p>
    </div>

    <div class="text-left text-sm border-b border-gray-300 py-3">
      <p><b>Mengubah petunjuk jawaban:</b></p>
      <li class="list-none py-2 flex items-center">
        <div class="tile w-10 h-10 mr-1.5 text-2xl">I</div>
        : Kondisi Awal
      </li>
      <li class="list-none py-2 flex items-center">
        <div class="tile absent border-none w-10 h-10 mr-1.5 text-2xl">A</div>
        : klik satu kali
      </li>
      <li class="list-none py-2 flex items-center">
        <div class="tile present border-none w-10 h-10 mr-1.5 text-2xl">P</div>
        : klik dua kali
      </li>
      <li class="list-none py-2 flex items-center">
        <div class="tile correct border-none w-10 h-10 mr-1.5 text-2xl">C</div>
        : klik tiga kali
      </li>
    </div>

    <div class="text-left text-sm py-3">
      <p>
        Github repo:
        <a
          class="hyperlink"
          href="https://github.com/uthadehikaru/wordle-helper"
          target="_blank"
          >https://github.com/uthadehikaru/wordle-helper</a
        >
      </p>
    </div>
  </div>
</template>

<script setup lang="ts">
defineEmits<{
  (e: "close"): void;
}>();
</script>
