<template>
  <q-tooltip
    content-class="tooltip tooltip-arrow-right-bottom"
    anchor="top middle"
    self="bottom middle"
    :offset="[15, 15]"
    max-width="380px"
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
$box-shadow: 0px 0px 30px 0 rgba(0, 0, 0, 0.2);

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
    transform: translateX(-50%) rotate(-45deg) skew(-20deg, -20deg);

    // top arrows
    [class*="tooltip-arrow-top"] & {
      top: 0;
    }
    .tooltip-arrow-top & {
      left: 50%;
    }
    .tooltip-arrow-top-left & {
      left: 50px;
    }
    .tooltip-arrow-top-right & {
      right: 23px;
    }

    // bottom arrows
    [class*="tooltip-arrow-bottom"] & {
      bottom: 0;
    }
    .tooltip-arrow-bottom & {
      left: 50%;
    }
    .tooltip-arrow-bottom-left & {
      left: 50px;
    }
    .tooltip-arrow-bottom-right & {
      right: 40px;
    }

    // left arrows
    [class*="tooltip-arrow-left"] & {
      transform: translateY(-50%) rotate(45deg) skew(-20deg, -20deg);
      left: 0;
    }
    .tooltip-arrow-left & {
      top: 50%;
    }
    .tooltip-arrow-left-top & {
      top: 50px;
    }
    .tooltip-arrow-left-bottom & {
      bottom: 20px;
    }

    // right arrows
    [class*="tooltip-arrow-right"] & {
      transform: translateY(-50%) rotate(45deg) skew(-20deg, -20deg);
      right: 0;
    }
    .tooltip-arrow-right & {
      top: 50%;
    }
    .tooltip-arrow-right-top & {
      top: 50px;
    }
    .tooltip-arrow-right-bottom & {
      bottom: 20px;
    }
  }
}
</style>
