<!-- 1.-  Input de texto simple
Enunciado: Crea un componente que tenga un campo de texto donde el usuario pueda escribir su nombre. El nombre debe mostrarse de forma dinámica en un h1 usando v-model. -->

<template>
    <input v-model="user" type="text" placeholder="Ingresa tu nombre"/>
    <h1>{{ user }}</h1>
</template>

<script>
export default {
    name: 'Actividad1',
    data() {
        return {
            user:''
        };
    }
};
</script>

<style scoped>
</style>