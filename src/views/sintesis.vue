<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    .row
      .col-12
        img(src="@/assets/curso/sintesis/img1.png")
      .row.justify-content-center
        .col-10.bg-color21
          .p-4
            p.mb-0 Los frameworks como Hibernate facilitan la conexión y manipulación de bases de datos relacionales ya que vienen configurados y optimizados para abstraer la complejidad propia de las bases de datos y permiten al desarrollador enfocarse en trabajar únicamente con el paradigma orientado a objetos. Adicionalmente una vez configurado el Framework facilita la realización de todo tipo de operación DML (SELECT, INSERT, UPDATE y DELETE) acelerando la velocidad en la que se pueden desarrollar aplicaciones JAVA que gestionan bases de datos relacionales. A continuación, se muestra un mapa conceptual de los elementos más importantes desarrollados en el primer apartado de este componente:
      .row.bg-color15
        .col-12
          .p-4
            img(src="@/assets/curso/sintesis/img1.svg" style="width: 1200px").m-auto(data-aos="slide-right")

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
