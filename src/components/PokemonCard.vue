<template>
  <div
    class="w-[220px] bg-[#f0f0f3] rounded-[20px] p-6 shadow-[8px_8px_16px_#d1d1d4,-8px_-8px_16px_#ffffff] transition-all duration-300 ease-in-out cursor-pointer hover:-translate-y-1 hover:shadow-[12px_12px_24px_#d1d1d4,-12px_-12px_24px_#ffffff] group"
  >
    <!-- Header -->
    <div class="text-center mb-5">
      <span
        class="inline-block px-4 py-1.5 bg-[#e8e8eb] rounded-2xl shadow-[inset_3px_3px_6px_#d1d1d4,inset_-3px_-3px_6px_#ffffff] text-[11px] font-semibold uppercase text-gray-500 tracking-wide"
      >
        {{ tipo }}
      </span>
    </div>

    <!-- Body -->
    <div class="text-center">
      <img
        :src="sprite"
        :alt="nombre"
        class="w-[140px] h-[140px] object-contain mb-4 mx-auto drop-shadow-md transition-transform duration-300 group-hover:scale-105"
      />
      <h3 class="text-xl font-bold text-gray-700 capitalize tracking-wide">
        {{ nombre }}
      </h3>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  nombre: string
  sprite: string
  tipo: string
}>()
</script>
