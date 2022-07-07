<template>
  <q-tooltip
    content-class="tooltip"
    max-width="400px"
    anchor="top middle"
    self="bottom middle"
    offset="[10, 10]"
    transition-show="scale"
    transition-hide="scale"
  >
    <div class="tooltip-text bg-grey-10 text-body2 text-justify no-scroll relative-position">
      <slot />
    </div>
    <div class="tooltip-arrow bg-grey-10 absolute"></div>
  </q-tooltip>
</template>

<script>
export default {
  data() {
    return {
      showing: true,
    };
  },
};
</script>

<style lang="scss">
$box-shadow: 0px 0px 30px 0 rgba(0, 0, 0, 0.5);

.tooltip {
  box-shadow: $box-shadow;
  background: transparent;
  border-radius: 75px;
  overflow: visible;
  padding: 0;

  &-text {
    z-index: 10;
    box-shadow: $box-shadow;
    border-radius: 75px;
    padding: 30px 30px 10px 30px;
  }

  &-arrow {
    z-index: 5;
    width: 30px;
    height: 30px;
    bottom: 0;
    left: 50%;
    transform: translateX(-50%) rotate(-45deg) skew(-20deg, -20deg);
  }
}
</style>
