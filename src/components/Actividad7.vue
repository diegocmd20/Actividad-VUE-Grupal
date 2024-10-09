<!-- 7.-  Enlace dinámico al atributo src de una imagen
Enunciado: Crea un componente que muestre una imagen con un src dinámico. El enlace de la imagen debe estar almacenado en el data del componente y cambiarse mediante v-bind. -->
<template>
  <div>
    <form>
      <label>ingrese la url de su imagen: </label>
      <input v-model="urlImagen" />
    </form>
    <img :src="urlImagen" />
  </div>
</template>

<script>
export default {
  name: 'Actividad7',
  data() {
    return {
      urlImagen:'',
    };
  }
};
</script>

<style scoped>
</style>