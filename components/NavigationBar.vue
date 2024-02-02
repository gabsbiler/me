<script setup lang="ts">
const routes = [
    {
        to: '/services',
        name: 'Services'
    },
    {
        to: '/projects',
        name: 'Projects'
    },
    {
        to: '/blog',
        name: 'Blog'
    },
    {
        to: '/about',
        name: 'About Me'
    }
]
</script>
<template>
    <VCard class="my-6">
        <VCardText class="d-flex justify-space-between align-center">
            <div>
                <h5 class="text-h5">
                    <NuxtLink to="/">Gabriel Biler</NuxtLink>
                </h5>
            </div>
            <div class="d-flex flex-row" >
                <div v-for="route in routes" class="mx-2">
                    <NuxtLink :to="route.to">{{route.name}}</NuxtLink>
                </div>
            </div>
            <div>
                <VBtn>Hire Me</VBtn>
            </div>
        </VCardText>
    </VCard>
</template>
