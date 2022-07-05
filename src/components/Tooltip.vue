<template>
  <q-tooltip class="tooltip bg-grey-10 text-body1">
    <slot />
  </q-tooltip>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.tooltip {
  box-shadow: 0 0 30px 0 rgba(0, 0, 0, 0.5);
  border-radius: 50px;
}
</style>
