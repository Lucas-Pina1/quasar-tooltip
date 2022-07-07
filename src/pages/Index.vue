<template>
  <q-page class="flex flex-center">
    <q-icon name="help" size="xs" class="cursor-pointer">
      <tooltip>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque
          inventore ducimus quod incidunt ratione tempore accusantium provident
          dolor asperiores amet dolore repudiandae iste natus eveniet quae
          perspiciatis cumque, odit dicta.
        </p>
        <p>
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Tempora quae
          unde dolor? Magni, accusantium omnis? Recusandae blanditiis nisi nulla
          delectus placeat perspiciatis nam, tenetur sunt totam animi dolores
          non. Architecto?
        </p>
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
