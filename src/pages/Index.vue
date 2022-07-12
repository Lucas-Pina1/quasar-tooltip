<template>
  <q-page class="flex flex-center">
    <div>
      <q-icon name="help" size="xs" class="cursor-pointer" color="grey">
        <tooltip>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque
            inventore ducimus quod incidunt ratione tempore accusantium
            provident
          </p>
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Tempora
            quae unde dolor? Magni, accusantium omnis? Recusandae blanditiis
            nisi nulla
          </p>
        </tooltip>
      </q-icon>
    </div>
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
