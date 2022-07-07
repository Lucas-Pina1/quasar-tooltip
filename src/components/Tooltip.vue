<template>
  <q-tooltip
    content-class="tooltip"
    anchor="top middle"
    self="bottom middle"
    :offset="[15, 15]"
    max-width="350px"
    transition-show="scale"
    transition-hide="scale"
  >
    <div
      class="tooltip-text bg-grey-10 text-caption text-justify relative-position"
    >
      <slot />
    </div>
    <div class="tooltip-arrow bg-grey-10 absolute"></div>
  </q-tooltip>
</template>

<script>
export default {};
</script>

<style lang="scss">
$box-shadow: 0px 0px 30px 0 rgba(0, 0, 0, 0.5);

.tooltip {
  box-shadow: $box-shadow;
  background: transparent;
  border-radius: 25%;
  overflow: visible;
  padding: 0;

  &-text {
    z-index: 10;
    box-shadow: $box-shadow;
    border-radius: 25%;
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
