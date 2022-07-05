<template>
  <q-page class="flex flex-center">
    <q-icon
      name="help"
      size="xs"
      class="cursor-pointer"
    >
      <tooltip
        :model-value="true"
      >
      Teste teste
      </tooltip>
    </q-icon>
  </q-page>
</template>

<script>
import Tooltip from '../components/Tooltip.vue';

export default {
  name: 'PageIndex',
  components: {
    Tooltip,
  },
};
</script>
