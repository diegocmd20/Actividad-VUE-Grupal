<!-- Made by Luis Suarez -->


<!-- 6.-  Enlace dinámico al atributo href de un enlace
Enunciado: Crea un componente que tenga un enlace (a) donde el href sea dinámico. El valor del enlace debe estar en el data del componente y cambiarse mediante v-bind. -->

<template>
    <div>
      <h2>Enlace Dinámico</h2>
      <p>
        <a :href="linkUrl" target="_blank">{{ linkText }}</a>
      </p>
      <button @click="changeLink">Cambiar Enlace</button>
    </div>
  </template>
  <script>
  export default {
    data() {
      return {
        linkUrl: 'https://google.com',
        linkText: 'Sitio oficial de Google'
      }
    },
    methods: {
      changeLink() {
        if (this.linkUrl === 'https://google.com') {
          this.linkUrl = 'https://youtube.com';
          this.linkText = 'Sitio Oficial De Youtube';
        } else {
          this.linkUrl = 'https://google.com';
          this.linkText = 'Sitio Oficial de Google';
        }
      }
    }
  }
  </script>