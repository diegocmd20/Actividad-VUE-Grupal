<!-- 2.-  Selección de opción en un dropdown
Enunciado: Crea un componente con un menú desplegable (select) que permita al usuario elegir una opción de color. Muestra el color seleccionado dinámicamente en un párrafo debajo. -->

<template>
    <select v-model="color">
        <option value="background-color:red;">Rojo</option>
        <option value="background-color:green;">Verde</option>
        <option value="background-color:yellow;">Amarillo</option>
    </select>
    <p :style="color">Texto</p>
</template>

<script>
export default {
    name: 'Actividad2',
    data() {
        return {
            color:'background-color:#242424;'
        };
    }
};
</script>

<style scoped>
</style>