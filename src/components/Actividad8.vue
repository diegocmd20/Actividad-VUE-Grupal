<!-- 8.- Clases dinámicas con v-bind:class
Enunciado: Crea un componente que tenga un botón. El botón debe tener una clase CSS dinámica que cambie según un valor booleano en el data. Usa v-bind:class para aplicar la clase condicionalmente. -->
<template>
  <div>
    <button @click="selector=!selector" :class="selector ? clase1:clase2"></button>
  </div>
</template>

<script>
export default {
  name: 'Actividad8',
  data() {
    return {
      selector:false,
      clase1:'red',
      clase2:'blue'
    };
  }
};
</script>

<style scoped>
.red{
  background-color: red
}
.blue{
  background-color: blue;
}
</style>