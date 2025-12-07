<template>
  <div class="min-h-screen bg-[#f0f0f3] flex items-center justify-center p-6">
    <div class="container max-w-6xl">
      <!-- Header Neumorphic -->
      <div
        class="bg-[#f0f0f3] rounded-3xl shadow-[8px_8px_16px_#d1d1d4,-8px_-8px_16px_#ffffff] transition-all duration-300 hover:shadow-[12px_12px_20px_#d1d1d4,-12px_-12px_20px_#ffffff] p-12 mb-16 text-center"
      >
        <h1 class="text-5xl font-bold text-gray-800 mb-4 tracking-tight">🎮 Pokémon Cards Game</h1>
        <p class="text-lg text-gray-600 font-medium">Mi primer componente Vue 3</p>
      </div>

      <!-- Cards Grid -->
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 justify-items-center">
        <PokemonCard
          v-for="pokemon in pokemons"
          :key="pokemon.nombre"
          :nombre="pokemon.nombre"
          :sprite="pokemon.sprite"
          :tipo="pokemon.tipo"
        />
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import PokemonCard from './components/PokemonCard.vue'

const pokemons = [
  {
    nombre: 'Pikachu',
    sprite:
      'https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/official-artwork/25.png',
    tipo: 'electrico',
  },
  {
    nombre: 'Charmander',
    sprite:
      'https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/official-artwork/4.png',
    tipo: 'fuego',
  },
  {
    nombre: 'Squirtle',
    sprite:
      'https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/official-artwork/7.png',
    tipo: 'agua',
  },
]
</script>
