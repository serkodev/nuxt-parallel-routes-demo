<script setup lang="ts">
definePageMeta({
    alias: '/category/:type'
})

const a = ref()
onMounted(() => {
    a.value = Math.random()
})
</script>

<template>
    <div style="display: flex; gap: 24px;">
        <div style="display: flex; flex-direction: column;">
            category [type]: {{ useRoute().params.type }}
            rnd: {{ a }}
            
            <!-- page: -->
            <NuxtLink to="/thread/1">1</NuxtLink>
            <NuxtLink to="/thread/2">2</NuxtLink>
        </div>

        <NuxtPage />
    </div>
</template>
