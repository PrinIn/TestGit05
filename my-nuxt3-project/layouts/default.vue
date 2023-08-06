<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 flex justify-between">
                <NuxtLink to="/" class="font-bold">Four Archons</NuxtLink>
                <ul class="flex gap-4">
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="/gyffindor">Gyffindor</NuxtLink></li>
                    <li><NuxtLink to="/hufflepuff">Hufflepuff</NuxtLink></li>
                    <li><NuxtLink to="/ravenclaw">Ravenclaw</NuxtLink></li>
                    <li><NuxtLink to="/slytherin">slytherin</NuxtLink></li>
                </ul>
            </nav>
        </header>

        <!-- page content go here -->
        <div class="container mx-auto p-4">
            <slot />
        </div>
    </div>
</template>

<style scoped>
    .router-link-exact-active {
        color: #a1b412;
    }
</style>