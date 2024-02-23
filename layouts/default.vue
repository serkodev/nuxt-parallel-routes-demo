<template>
    <div style="display: flex; gap: 12px;">
        <div>
            <div style="display: flex; gap: 12px;">
                <NuxtLink to="/home">Home</NuxtLink>
                <NuxtLink to="/bookmark">Bookmark</NuxtLink>
            </div>
            <LeftSideView />
        </div>

        <div style="background-color: bisque; flex: 1;">
            <TopicView />
        </div>

        <!-- XXX: prevent not render on the first route (nuxt #25069) -->
        <div style="display: none;"><slot /></div>
    </div>
</template>
