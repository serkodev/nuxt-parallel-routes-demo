<script setup lang="ts">
import HomeList from './HomeList.vue'
import BookmarkList from './BookmarkList.vue'

const route = useRoute()

const leftSideView = ref(route.name)

const sideViews = {
  home: HomeList,
  bookmark: BookmarkList,
  topic: HomeList,
}

watch(() => route.name, (newName) => {
  if (newName === 'topic')
    return
  leftSideView.value = newName
})
</script>

<template>
  <component :is="(sideViews as any)[leftSideView!]" />
</template>
