<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
  
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span
          i.fas.fa-info
      h1 Introducción
    .margin-n.bg-intro.p-5.mb-5
      .row.justify-content-center.mb-5
        .col-lg-4.col-8(data-aos="fade-right").mb-lg-0.mb-3: img(src='@/assets/curso/temas/intro/1.png', alt='')
        .col-lg-7(data-aos="fade-left")
          .tarjeta.bg-white.p-5.tarjeta-intro 
            p.mb-4 Este nivel de formación bilingüe se enfoca en narrar recuentos anecdóticos y experiencias de vida; para esto, se necesita saber usar los tiempos 
              span.r--1 presente perfecto y pasado simple, 
              | ya que  estos se complementan para contar cabalmente una historia.  También se debe aprender a usar 
              span.r--1 los adverbios de modo, 
              | útiles para decir cómo o de qué manera se hicieron las cosas, y a usar las 
              span.r--1 frases exclamativas, 
              | las cuales ayudan a expresar sorpresa, conmoción o una emoción fuerte sobre lo que se está narrando. Partiendo de lo anterior, le damos la bienvenida al estudio de este componente formativo y, para comenzar, se le invita a explorar el video que se presenta a continuación:
            .tarjeta-intro__icon1: img(src='@/assets/curso/portada/a4.svg', alt='')
            .tarjeta-intro__icon2: img(src='@/assets/curso/portada/a5.svg', alt='')
            .tarjeta-intro__cta.mx-5
              a.anexo.my-4.mb-lg-0(:href="obtenerLink('downloads/doc1.pdf')" target="_blank" style='background-color: #3c3fa7')
                .anexo__icono
                  img(src="@/assets/template/icono-pdf.svg")
                .anexo__texto()
                  p
                    span.r--2.fw-normal #[b Anexo.] Si desea practicar, el siguiente PDF presenta los textos del siguiente video, tanto en inglés como en español.
    figure
      .video
        iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    
</template>

<script>
export default {
  name: 'Introduccion',
  data: () => ({
    // variables de vue
  }),
}
</script>

<style lang="sass">
.bg-intro
  background-image: url('../assets/curso/temas/intro/bg-intro.png')
  background-repeat: no-repeat
  background-size: cover
  background-position: center
</style>
