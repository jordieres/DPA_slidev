<template>
  <div class="slidev-layout default">
    <div class="top-banner">
      <img src="/images/upm-header.png">
      <div class="banner-title">
        {{ slide.$frontmatter.title }}
      </div>
    </div>

    <div class="default-content">
      <slot />
    </div>
  </div>
</template>

<style scoped>
.center-layout {
  height: 100%;
  display: flex;
  flex-direction: column;
}

.slide-header {
  flex: 0 0 auto;
}

.header-image {
  width: 100%;
  display: block;
}

.center-content {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>