<template>
    <div class="overflow-hidden bg-white py-24 sm:py-32">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="mx-auto grid max-w-2xl grid-cols-1 gap-x-8 gap-y-16 sm:gap-y-20 lg:mx-0 lg:max-w-none lg:grid-cols-2">
          <div class="lg:pr-8 lg:pt-4">
            <div class="lg:max-w-lg">
              <h2 class="text-base font-semibold leading-7 text-indigo-600">Muhammad Sadad</h2>
              <p class="mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">Erigo Apparel</p>
              <p class="mt-6 text-lg leading-8 text-gray-600">ERIGO is a local brand, the pride of Indonesia. ERIGO is a fashion brand founded by Muhammad Sadad in 2011. This local brand focuses on streetwear fashion that can be worn by men and women in Indonesia and globally. ERIGO has succeeded in becoming a local brand that is selling well in the market and has even begun to go global.</p>
              <dl class="mt-10 max-w-xl space-y-8 text-base leading-7 text-gray-600 lg:max-w-none">
                <div v-for="feature in features" :key="feature.name" class="relative pl-9">
                  <dt class="inline font-semibold text-gray-900">
                    <component :is="feature.icon" class="absolute left-1 top-1 h-5 w-5 text-indigo-600" aria-hidden="true" />
                    {{ feature.name }}
                  </dt>
                  {{ ' ' }}
                  <dd class="inline">{{ feature.description }}</dd>
                </div>
              </dl>
            </div>
          </div>
          <img src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Product screenshot" class="w-[48rem] max-w-none rounded-xl shadow-xl ring-1 ring-gray-400/10 sm:w-[57rem] md:-ml-4 lg:-ml-0" width="2432" height="1442" />
        </div>
      </div>
    </div>
  </template>

<script setup>
import { ShoppingBagIcon, LockClosedIcon, ServerIcon } from '@heroicons/vue/20/solid'

const features = [
  {
    name: 'T-Shirt',
    description:
      'pakaian yang nyaman dan serbaguna. Biasanya terbuat dari bahan katun ringan yang cocok untuk digunakan dalam berbagai kesempatan. Kaos memiliki leher bulat dan lengan pendek.',
    icon: ShoppingBagIcon,
  },
  {
    name: 'Outerwear',
    description: 'pakaian yang dirancang untuk dikenakan di atas pakaian biasa guna memberikan perlindungan dari elemen cuaca yang tidak nyaman seperti angin, hujan, atau dingin.',
    icon: LockClosedIcon,
  },
  {
    name: 'Pants',
    description: 'pakaian yang dikenakan di bagian bawah tubuh, biasanya dari pinggang hingga pergelangan kaki.',
    icon: ServerIcon,
  },
]
</script>

<!-- <style scoped>
    h2 {
        margin-bottom: 20px;
        font-size: 36px;
    }
    p {
        margin: 20px 0;
    }
</style> -->