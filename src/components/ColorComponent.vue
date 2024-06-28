<script setup>
import { ref } from 'vue';
const colorFondo = ref('#000000'); // Color default value
const colortext = ref('#ffffff'); // Color default value
</script>
<template>
  <div class="wrapper">
    <div class="cube">
      <p>Color</p>
    </div>
    <p>
    color de fondo:
    <input type="color" v-model="colorFondo">
    </p>

    <p>
    color de texto:
    <input type="color" v-model="colortext">
    </p>
    
  
  </input>
   
  </div>
</template>

<style scoped>
.cube {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 20px;
  height: 80px;
  width: 80px;
  background: v-bind(colorFondo);
  color: v-bind(colortext);
  font-weight: 900;
}
</style>
