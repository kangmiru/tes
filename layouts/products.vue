<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 flex justify-between border-t-2">
            <NuxtLink to="/products" class="font-bold">Erigo Merch</NuxtLink>
                <ul class="flex gap-10">
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="/about">About</NuxtLink></li>
                    <li><NuxtLink to="/products">Products</NuxtLink></li>
                </ul>
            </nav>      
        </header>
        
        <!-- output the page content -->
        <div class="container mx-auto p-6">
            <slot />
        </div>
    </div>
    <footer class="bg-gray-900 text-white text-center p-6">
        &copy; 2023 Erigo Website. All rights reserved.
    </footer>
</template>

<style scoped> 
    .router-link-exact-active {
        color: #12b488;
    }
</style>