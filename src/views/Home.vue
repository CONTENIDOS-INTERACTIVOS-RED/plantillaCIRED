<template lang="pug">
.curso-container.d-flex.flex-column.min-vh-100
  .container.flex-grow-1
    .bg-white.mt-5
      .row.g-0
        //- Columna izquierda con imagen
        .col-md-6.imagen-section
          img.img-fluid(
            src="@/assets/portada/chica-laptop.png"
            alt="Estudiante virtual"
            style="max-width: 672px;"
          )
        //- Columna derecha con información
        .col-md-6.info-section
          .content-wrapper.p-5.text-start
            img.logo(
              src="@/assets/portada/logo-xs.png"
              alt="Logo Tecnológica del Oriente"
            )
            h1.mb-5 PREPARACIÓN INTEGRAL PARA EL TRABAJO EN MODALIDAD VIRTUAL
            p.descripcion.mb-4
              | Este programa de formación está diseñado para equiparte con las
              | habilidades y herramientas esenciales para desenvolverte con éxito
              | en entornos digitales. A lo largo del curso, aprenderás a gestionar
              | tu tiempo y tu aprendizaje de manera autónoma, dominarás el uso de
              | plataformas LMS y herramientas digitales, y desarrollarás
              | competencias clave para el manejo ético de la información.

            p #[strong ¡Prepárate para afrontar los retos del trabajo virtual con confianza y eficacia!]
            .button-container
              button.btn-iniciar
                | INICIAR 
                i.fas.fa-arrow-right

  //- Footer
  footer.footer.bg-white
    .container.px-4.py-5
      .row.justify-content-start.align-items-center
        .col-lg-auto
          img.logo-footer(
            src="@/assets/portada/logo-footer.png"
            alt="Logo Tecnológica del Oriente"
          )
        .col-lg
          p.footer-text.mb-0 Este material puede ser distribuido, copiado y exhibido por terceros si se muestra en los créditos. No se puede obtener ningún beneficio comercial y las obras derivadas tienen que estar bajo los mismos términos de la licencia que el trabajo original.
</template>

<script>
export default {
  name: 'Home',
}
</script>

<style scoped>
.curso-container {
  background-color: #80a5be;
}

.info-section {
  position: relative;
  min-height: 100%;
  display: flex;
  flex-direction: column;
  padding: 2rem;
}

.content-wrapper {
  display: flex;
  flex-direction: column;
  height: 100%;
}

.button-container {
  margin-top: auto;
  text-align: right;
}

.btn-iniciar {
  display: inline-block;
  /* Aquí tus estilos existentes para el botón */
}

.home {
  padding: 20px;
  text-align: center;
}

h1 {
  color: #2c3e50;
}

.logo {
  height: 40px;
  width: auto;
  margin-bottom: 1.5rem;
  object-fit: contain;
  align-self: flex-start; /* Asegura alineación izquierda incluso en contenedor flex */
}

.logo-footer {
  height: 30px; /* Ajusta según necesites */
  width: auto;
  object-fit: contain;
}

.footer {
  margin-top: auto; /* Empuja el footer al fondo */
  width: 100%;
}
</style>
