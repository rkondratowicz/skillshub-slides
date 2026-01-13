<template>
  <div class="slidev-layout default">
    <div class="my-auto w-full">
      <slot />
    </div>
    <img src="/assets/kainos_logo.png" alt="Kainos Logo" class="kainos-logo" />
  </div>
</template>

<style scoped>
.slidev-layout.default :deep(h1),
.slidev-layout.default :deep(h2),
.slidev-layout.default :deep(h3) {
  font-weight: 700;
}

.slidev-layout.default :deep(h1) {
  margin-bottom: 2rem;
}

.kainos-logo {
  position: absolute;
  bottom: 20px;
  right: 20px;
  height: 25px;
  width: auto;
}
</style>
