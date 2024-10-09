<!-- 3.- Checkbox con estado activo/inactivo
Enunciado: Crea un componente que tenga un checkbox para indicar si un usuario está activo o inactivo. Muestra un mensaje que cambie dinámicamente según el estado del checkbox. -->

<template>
  <div>
    <label for="">el usuario esta activo? </label>
    <input type="checkbox" v-model="usuarioActivo">
    <p v-if="usuarioActivo">efectivamente, el usuario se encuenta activo</p>
  </div>
</template>

<script>
export default {
  name: 'Actividad3',
  data() {
    return {
      usuarioActivo: false,
    };
  }
};
</script>

<style scoped>
</style>