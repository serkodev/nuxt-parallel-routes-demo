<script setup lang="ts">
const route = useRoute()
const id = ref(route.params.id)

watch(() => route.params.id, (value) => {
    if (value)
        id.value = value
})
</script>

<template>
    <div>Topic</div>
    <div>id: {{ id }}</div>
</template>
