<template>
    <div>
        <header class="shadow-sm bg-white">
      <nav class="container mx-auto p-4 flex justify-between items-center">
        <NuxtLink to="/" class="font-bold text-2xl">Erigo</NuxtLink>
        <ul class="flex gap-16">
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/products">Products</NuxtLink></li>
        </ul>
        <div class="flex items-center">
          <p class="mr-4">Color Mode:</p>
          <select v-model="colorMode.preference" class="border w-24 h-8 dark:bg-gray-900 dark:text-white dark:border-gray-700">
            <option value="system">System</option>
            <option value="light">Light</option>
            <option value="dark">Dark</option>
          </select>
        </div>
      </nav>
    </header>
  </div>

        <!-- output the page content -->
        <div class="container mx-auto p-4">
            <slot />
        </div>
    
</template>

<script setup>
const colorMode = useColorMode()
</script>

<style lang="postcss"> 
    .router-link-exact-active {
        color: #12b488;
    }  
    body {
        @apply min-h-screen bg-white dark:bg-gray-800 dark:text-gray-200;
      } 
</style>