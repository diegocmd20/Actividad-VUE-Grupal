<!-- 5.-  Textarea con descripción
Enunciado: Crea un componente que tenga un textarea donde el usuario pueda escribir una descripción. Muestra la descripción introducida en tiempo real en un párrafo debajo del textarea. -->

<template>
    <textarea v-model="areaTexto" placeholder="Ingresa la descripcion"></textarea>
    <p><strong>{{ areaTexto }}</strong></p>
</template>

<script>
export default {
    name: 'Actividad5',
    data() {
        return {
            areaTexto: ''
        };
    }
};
</script>

<style scoped>
</style>