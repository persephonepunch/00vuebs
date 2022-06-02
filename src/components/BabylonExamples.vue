<template>
<h3>Babylon</h3>
<Canvas>

</Canvas>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { CustomLoaders } from '@/BabylonExamples/CustomLoaders';

export default defineComponent({
  name: 'BabylonExamples',
  mounted(){
    const canvas = document.querySelector("canvas")!;
    new CustomLoaders(canvas);
  }
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
canvas {
  width:70%;
  height:70%;
}
</style>
