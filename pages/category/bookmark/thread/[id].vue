<script setup lang="ts">
definePageMeta({
    alias: '/thread/:id'
})
</script>

<template>
    <div>
        thread [id]: {{ useRoute().params.type }}
        thread [id]: {{ useRoute().params.id }}
    </div>
</template>
