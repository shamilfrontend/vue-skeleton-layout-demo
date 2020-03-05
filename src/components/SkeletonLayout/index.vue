<template>
  <div
    class="skeleton-layout"
    :style="{ color: bgColor }"
  >
    <slot />
  </div>
</template>

<script>
import SkeletonRow from './components/SkeletonRow/index.vue';
import SkeletonCol from './components/SkeletonCol/index.vue';
import SkeletonImage from './components/SkeletonImage/index.vue';

export { SkeletonRow, SkeletonCol, SkeletonImage };

export default {
  name: 'SkeletonLayout',

  props: {
    bgColor: {
      type: String,
      default: '#f3f3f3',
    },
  },
};
</script>

<style lang="scss" scoped>
@keyframes flicker {
  0% {
    transform: translateX(-80%);
  }

  100% {
    transform: translateX(80%);
  }
}

.skeleton-layout {
  position: relative;

  &::after {
    content: '';
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    z-index: 5;
    background-image: linear-gradient(
      90deg,
      transparent 40%,
      currentColor 50%,
      transparent 60%
    );
    opacity: 0.5;
    animation: flicker 1.5s infinite;
  }
}
</style>
