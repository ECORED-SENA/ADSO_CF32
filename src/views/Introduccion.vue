<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
  
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span
          i.fas.fa-info
      h1 Introducción
    p.mb-5 Vamos a comenzar el presente componente formativo con un video donde se describe de una manera general la temática a tratar:
    .row.bg-color1
      .col-12.px-5
        figure.mb-5
          .video
            iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
        .row.align-items-center
          .col-lg-6
            img(src="@/assets/curso/intro/img1.png").m-auto
          .col-lg-6
            .row
              .col-12
                .p-4.bg-color2
                  p Es en este contexto donde aparecen frameworks como Hibernate y Sprint para facilitar el proceso de transformación de información requerido entre el mundo de las bases de datos relacionales, la lógica de negocio y el mundo de la programación orientada a objetos.


</template>

<script>
export default {
  name: 'Introduccion',
  data: () => ({
    // variables de vue
  }),
}
</script>

<style lang="sass"></style>
