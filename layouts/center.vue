<template>
  <div class="slidev-layout center">
    <div class="my-auto w-full text-center">
      <slot />
    </div>
  </div>
</template>

<style scoped>
.slidev-layout.center {
  @apply h-full grid;
}

.slidev-layout.center :deep(h1) {
  @apply text-6xl leading-20;
  font-weight: 700;
}

.slidev-layout.center :deep(h1 + p) {
  @apply -mt-2 opacity-50 mb-4;
}

.slidev-layout.center :deep(p + h2),
.slidev-layout.center :deep(ul + h2),
.slidev-layout.center :deep(table + h2) {
  @apply mt-10;
}
</style>
