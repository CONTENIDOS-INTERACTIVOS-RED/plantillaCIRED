<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(:titulo="'FUNDAMENTACIÓN JURÍDICA - unidad 1'" :subTitulo="'INTRODUCCIÓN'")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .row.justify-content-between.mb-5
      .col-md-6.col-lg-7
        p Desde los inicios de la humanidad, las reglas han sido un elemento fundamental para el desarrollo de las sociedades. El Derecho, en este contexto, se presenta como una herramienta indispensable para el buen funcionamiento de la convivencia. En esta primera unidad, se profundizará en el concepto de Derecho, su propósito y origen, así como en el proceso de creación de normas que regulan nuestras actividades diarias, las relaciones entre individuos y el Estado, y las normas que operan en el ámbito global.
      .col-md-6.col-lg-5
        //- .imagen-titulo--der debe ir acompañado de una de una de estas clases => 
        //- .color-primario, .color-secundario, .color-acento-contenido, .color-acento-botones
        .imagen-titulo--der.color-secundario
          figure
            img(src='@/assets/template/test-img.png', alt='Texto que describa la imagen')
            .imagen-titulo__titulo
              h4.m-0 Titulo de imagen
    .row.justify-content-between.mb-5
      .col-md-6.col-lg-7
        AcordionA(tipo="b")
          .row(titulo="Titulo item 1")
            .col
              p This is another paragraph. I think it needs to be added that the set of elements tested is not exhaustive in any sense. I have selected those elements for which it can make sense to write user style sheet rules, in my opionion.

          div(titulo="Titulo item 2")
            figure
              img(src='@/assets/template/img-placeholder.svg', alt='Texto que describa la imagen')
              figcaption Leyenda de la imagen
      .col-md-6.col-lg-5
        //- .imagen-titulo--der debe ir acompañado de una de una de estas clases => 
        //- .color-primario, .color-secundario, .color-acento-contenido, .color-acento-botones
        .imagen-titulo--der.color-secundario
          figure
            img(src='@/assets/template/test-img.png', alt='Texto que describa la imagen')
            .imagen-titulo__titulo
              h4.m-0 Titulo de imagen
</template>

<script>
export default {
  name: 'Tema1',
  data: () => ({}),

  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
}
</script>

<style lang="sass"></style>
