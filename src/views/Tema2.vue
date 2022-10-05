<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 2
      h1 #[em Present Perfect] (Presente perfecto)
    .row.justify-content-center.mb-5
      .col-lg-6(data-aos="fade-right")
        .tarjeta.p-4(style='background-color: #C4D1FF')
          div(style='background-color: #F0F4FF').p-2.mb-3
            p.text-center #[em We use Present Perfect for actions in the past which have a connection to the present, the time when these actions happened is not important.]
            img(src='@/assets/curso/temas/tema2/1.svg', alt='')
          p.text-center #[em We use the Present Perfect for recently completed actions.]
          img(src='@/assets/curso/temas/tema2/2.svg', alt='').mb-4
          div(style='background-color: #F0F4FF').p-2.mb-3
            p.text-center #[em We use Present Perfect for actions beginning in the past and still continuing.]
            img(src='@/assets/curso/temas/tema2/3.svg', alt='')
      .col-lg-6(data-aos="fade-left") 
        .contenedor-traductor(style='background-color: #fcf2ca').mb-5
          .contenedor-traductor__eng
            p.fst-italic The present perfect tense speaks of an action that took place in the past but still has some importance in the present tense, life experiences, and it focuses on a fact that has happened.
          .contenedor-traductor__esp(:class="{ mostrar: ocultarEsp}")
            //TODO Agregar traducción
            p 
          a.boton-traduccion(@click='ocultarEsp = !ocultarEsp' style='background-color: #fc5f65') Ver traducción
        img(src='@/assets/curso/temas/tema2/4.svg', alt='')
    p.text-center El siguiente video nos amplía la información sobre el uso del 
      span.r--1.fw-bold #[em Present perfect.]
    figure.mb-5
      .video
        iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    .row.justify-content-center.mb-5
      .col-lg-8
        a.anexo.my-4.mb-lg-0(href="" target="_blank" style='background-color: #3c3fa7')
                .anexo__icono
                  img(src="@/assets/template/icono-pdf.svg")
                .anexo__texto()
                  p
                    span.r--2.fw-normal #[b Anexo.] Si desea practicar, el siguiente PDF presenta los textos del video anterior, tanto en inglés como en español.
    .margin-n.p-5(style="background-color: #E1E8FF").mb-5
      .row.justify-content-center.mb-5
        .col-lg-9
          .tarjeta.bg-white.p-5.tarjeta-intro 
            h5.text-center
              span.r--1  #[em Thematic Dialogue]  / Diálogo temático
            p.mb-5.text-center #[em  A love story using the present perfect.]
            .row.justify-content-center.align-items-center.mb-5
              .col-lg-6.col-8.mb-lg-0.mb-3(data-aos="fade-right")
                img(src='@/assets/curso/temas/tema2/5.svg', alt='')
              .col-lg-6(data-aos="fade-left")
                  TarjetaAudio.no-input.mb-3(
                    texto="<b>Son:</b> Mom, tell me about you and dad. How has your love story been?"
                    :audio="require('@/assets/curso/audios/tema1/1.mp3')"
                    @audio-hover="mostrarIndicadorTarjetaAudio = false"
                    style='background-color: #cad3f2; border: 0px'
                  )
                  TarjetaAudio.no-input.mb-3(
                    texto="<b>Mom:</b> Well, son, he and I met at school, when we were 13, but we’ve been together since we were 18, when we fell in love. The next year, we got married, moved to the United States and lived abroad for over 20 years before coming back to our hometown."
                    :audio="require('@/assets/curso/audios/tema1/1.mp3')"
                    @audio-hover="mostrarIndicadorTarjetaAudio = false"
                    style='background-color: #fff0b5; border: 0px'
                  )
            .row.justify-content-center.align-items-center.mb-5
              .col-lg-6(data-aos="fade-left")
                  TarjetaAudio.no-input.mb-3(
                    texto="<b>Son:</b> You have known each other for almost your entire life."
                    :audio="require('@/assets/curso/audios/tema1/1.mp3')"
                    @audio-hover="mostrarIndicadorTarjetaAudio = false"
                    style='background-color: #cad3f2; border: 0px'
                  )
                  TarjetaAudio.no-input.mb-3(
                    texto="<b>Mom:</b> Yes, we have lived together for over 40 years and haven’t spent a single day apart."
                    :audio="require('@/assets/curso/audios/tema1/1.mp3')"
                    @audio-hover="mostrarIndicadorTarjetaAudio = false"
                    style='background-color: #fff0b5; border: 0px'
                  )
              .col-lg-6.col-8.mb-lg-0.mb-3(data-aos="fade-right")
                img(src='@/assets/curso/temas/tema2/6.svg', alt='')
            .tarjeta-intro__icon1: img(src='@/assets/curso/portada/a4.svg', alt='')
            .tarjeta-intro__icon2: img(src='@/assets/curso/portada/a5.svg', alt='')    
    .row.justify-content-center.mb-5
      .col-lg-5(data-aos="fade-right")
        div(style="background-color: #FCF2CA").p-3
</template>

<script>
export default {
  name: 'Tema2',
  data: () => ({
    ocultarEsp: true,
    dialogo: {
      personajes: [
        {
          nombre: 'Sonia',
          img: require('@/assets/curso/temas/tema1/son.svg'),
        },
        {
          nombre: 'Pedro',
          img: require('@/assets/curso/temas/tema1/mon.svg'),
        },
      ],
      dialogo: [
        {
          personaje: 'Sonia',
          textoIng:
            'And what has *** the most difficult moment in your marriage?',
          textoEsp: 'Yo necesito el libro de biologia y las diapositivas.',
          audio: require('@/assets/curso/audios/tema1/1.mp3'),
          palabra: 'been',
        },
        {
          personaje: 'Pedro',
          textoIng:
            'Probably, when your grandmother died, your dad’s mother. It is very sad to lose a loved one, and in times like those we *** supported each other as a couple. It hasn’t been easy being together for so long.',
          textoEsp: '',
          audio: require('@/assets/curso/audios/tema1/1.mp3'),
          palabra: 'have',
        },
      ],
    },
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
