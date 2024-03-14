<script setup lang="ts">
definePageMeta({
    alias: '/category/bookmark'
})
</script>

<template>
    <div style="display: flex; gap: 24px;">
        <div style="display: flex; flex-direction: column;">
            /bookmark~~~
            
            <!-- page: -->
            <NuxtLink to="/thread/4">3</NuxtLink>
            <NuxtLink to="/thread/5">4</NuxtLink>
        </div>

        <NuxtPage />
    </div>
</template>
