<template>
    <div style="display: flex; flex-direction: column; gap: 12px;">
        <div style="font-size: larger;">Home</div>
        <NuxtLink to="/topic/1">/topic/1</NuxtLink>
        <NuxtLink to="/topic/2">/topic/2</NuxtLink>
        <NuxtLink to="/topic/3">/topic/3</NuxtLink>
        <NuxtLink to="/topic/4">/topic/4</NuxtLink>
        <NuxtLink to="/topic/5">/topic/5</NuxtLink>
    </div>
</template>

<style scoped>
a {
    display: block;
    padding: 8px;
    background-color: aqua;
}
</style>
