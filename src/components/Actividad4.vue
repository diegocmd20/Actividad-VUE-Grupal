<!-- 4.-  Input de número con contador
Enunciado: Crea un componente que tenga un input de tipo número. El valor del input debe controlarse mediante v-model y mostrarlo en un párrafo. -->
<template>
  <div>
    <input type="number" v-model="contador">
    <p>{{ contador }}</p>
  </div>

</template>

<script>
export default {
  name: 'Actividad4',
  data() {
    return {
      contador:' ',
    };
  }
};
</script>

<style scoped>
</style>