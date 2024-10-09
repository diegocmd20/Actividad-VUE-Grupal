<!-- 8.- Clases dinámicas con v-bind:class
Enunciado: Crea un componente que tenga un botón. El botón debe tener una clase CSS dinámica que cambie según un valor booleano en el data. Usa v-bind:class para aplicar la clase condicionalmente. -->
<template>
  <select v-model="color">
      <option value="yellow">Amarillo</option>
      <option value="red">Rojo</option>
      <option value="green">Verde</option>
  </select>
  <!-- Data Bind de Class  -->
  <p :class="{red:color === 'red', yellow:color === 'yellow', green:color === 'green'}">Parrafo de Ejemplo {{ color }}</p> 
  <!-- Data Bind con Style -->
  <p :style="{color:color}">El color seleccionado es: {{ color }}</p>
  <!-- Data Bind más corto de clase -->
  <p :class="color">Texto de Ejemplo</p>
</template>
<script>
export default {
  name: 'Seleccion',
  data() {
      return {
          color: 'red',
      };
  }
};
</script>
<style scoped>
  .red{
      color: red;
  }
  
  .yellow{
      color: yellow;
  }
  .green{
      color: green;
  }
</style>