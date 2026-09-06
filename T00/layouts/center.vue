<script setup>
import { computed } from 'vue'
import { useSlideContext } from '@slidev/client'

const slide = useSlideContext()

const title = computed(() =>
  slide.$frontmatter?.title || ''
)
</script>

<template>
  <div class="slidev-layout center-layout">
    <div class="top-banner">
      <img src="/images/upm-header.png">
      <div class="banner-title">
        {{ slide.$frontmatter.title }}
      </div>
    </div>

    <div class="center-content">
      <slot />
    </div>
  </div>
</template>

<style scoped>

.slide-header {
  flex: 0 0 auto;
}

.center-layout {
  position: relative;
  width: 100%;
  height: 100%;
  padding: 0 !important;
  margin: 0;
  overflow: hidden;
}

.top-banner {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 90px;
  z-index: 10;
}

.top-banner img {
  display: block;
  width: 100%;
  height: auto;
}

.center-content {
  position: absolute;
  top: 80px;
  bottom: 0;
  left: 0;
  right: 0;
  padding: 5px;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 1;
}

.center-content :deep(p) {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
  margin: 0;
}

.center-content :deep(img) {
  max-width: 100%;
  max-height: 100%;
  width: auto;
  height: auto;
  object-fit: contain;
  display: block;
}

</style>
