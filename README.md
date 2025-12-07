# Pokémon Cards Component

Proyecto de componentes reutilizables de tarjetas Pokémon desarrollado con Vue 3, TypeScript y Tailwind CSS con diseño neumórfico elegante y minimalista.

## 🎮 Características

- ✨ Diseño neumórfico moderno y elegante
- 🎨 Paleta de colores claros y minimalista
- 🃏 Componente `PokemonCard` reutilizable
- 🚀 Props configurables (nombre, sprite, tipo)
- 💅 Estilos con Tailwind CSS puro
- 📱 Diseño responsive

## 🛠️ Tecnologías

- Vue 3 (Composition API)
- TypeScript
- Tailwind CSS v4
- Vite
- Pinia (State Management)
- Vitest (Testing)

## 📋 Recommended IDE Setup

[VS Code](https://code.visualstudio.com/) + [Vue (Official)](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur).

## 🌐 Recommended Browser Setup

- Chromium-based browsers (Chrome, Edge, Brave, etc.):
  - [Vue.js devtools](https://chromewebstore.google.com/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd) 
  - [Turn on Custom Object Formatter in Chrome DevTools](http://bit.ly/object-formatters)
- Firefox:
  - [Vue.js devtools](https://addons.mozilla.org/en-US/firefox/addon/vue-js-devtools/)
  - [Turn on Custom Object Formatter in Firefox DevTools](https://fxdx.dev/firefox-devtools-custom-object-formatters/)

## 📦 Project Setup

```sh
pnpm install
```

### Compile and Hot-Reload for Development

```sh
pnpm dev
```

### Type-Check, Compile and Minify for Production

```sh
pnpm build
```

### Run Unit Tests with [Vitest](https://vitest.dev/)

```sh
pnpm test:unit
```

### Lint with [ESLint](https://eslint.org/)

```sh
pnpm lint
```

## 🎯 Uso del Componente

```vue
<template>
  <PokemonCard
    nombre="Pikachu"
    sprite="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/official-artwork/25.png"
    tipo="electrico"
  />
</template>

<script setup lang="ts">
import PokemonCard from './components/PokemonCard.vue'
</script>
```

## 📚 Estructura del Proyecto

```
src/
├── components/
│   └── PokemonCard.vue    # Componente de tarjeta Pokémon
├── stores/                # Pinia stores
├── __tests__/            # Tests unitarios
├── App.vue               # Componente principal
├── main.ts               # Entry point
└── style.css             # Estilos globales
```

## 🎨 Conceptos Aplicados

- ✅ Componentes reutilizables
- ✅ Props y tipado con TypeScript
- ✅ Diseño neumórfico
- ✅ Tailwind CSS utility classes
- ✅ Organización del proyecto
- ✅ State management con Pinia

## 📄 License

MIT

