<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 1
      h1 #[em I have won the lotto twice!] (¡Yo he ganado la lotería dos veces!)
    .row.justify-content-center.align-items-center.mb-5
      .col-lg-7.mb-lg-0.mb-3(data-aos="fade-right")
        .contenedor-traductor(style='background-color: #fcf2ca')
          .contenedor-traductor__eng
            p.fst-italic The present perfect is the verb tense used to talk about life experiences, things that have been done and things that have happened. For this reason, we invite you to listen to the following dialogue between Sonia and Pedro using a clear and fluent conversation in this verb tense.
          .contenedor-traductor__esp(:class="{ mostrar: ocultarEsp}")
            p El presente perfecto es el tiempo verbal usado para hablar de experiencias de vida, de las cosas que se han hecho y que han pasado.   Por esta razón, se le invita a escuchar el siguiente diálogo entre Sonia y Pedro utilizando una conversación clara y fluida en este tiempo verbal.
          a.boton-traduccion(@click='ocultarEsp = !ocultarEsp' style='background-color: #fc5f65') Ver traducción
      .col-lg-4.col-8.mb-lg-0.mb-3(data-aos="fade-left"): img(src='@/assets/curso/temas/tema1/1.png', alt='')
    .bg-tema1.margin-n.p-5(style='background-color: #acade1').mb-5
      .row.justify-content-center.mb-5
        .col-lg-4.col-8.mb-lg-0.mb-3(data-aos="fade-right"): img(src='@/assets/curso/temas/tema1/2.jpg', alt='' style='border-radius: 10px')
        .col-lg-8(data-aos="fade-left")
          .contenedor-traductor(style='background-color: #fcf2ca').mb-5
            .contenedor-traductor__eng
              p.fst-italic Two or more people have a conversation in the present perfect when they talk about events that have been going on for a long time and can be repeated in the present, either sporadically or constantly, applying the grammatical rules.
            .contenedor-traductor__esp(:class="{ mostrar: ocultarEsp2}")

              //TODO Agregar texto traducido 


              p 
            a.boton-traduccion(@click='ocultarEsp2 = !ocultarEsp2' style='background-color: #fc5f65') Ver traducción
          .tarjeta.p-4(style='background-color: #ffdfe0')
            .row.justify-content-center.mb-5
              .col-lg-8.mb-lg-0.mb-3(data-aos="fade-right")
                .bg-white.p-3.h-100
                  SlyderE(indicadores="derecha")
                    div
                      p.text-center.fw-bold #[em Thematic Dialogue]  / Diálogo Temático
                      TarjetaAudio.no-input.mb-3(
                        texto="<b>Pedro:</b> Sonia, have you ever been on tv?"
                        :audio="require('@/assets/curso/audios/tema1/1.mp3')"
                        @audio-hover="mostrarIndicadorTarjetaAudio = false"
                        style='background-color: #cad3f2; border: 0px'
                      )
                      TarjetaAudio.no-input.mb-3(
                        texto="<b>Sonia:</b> Actually, yes, I have. I sang in the talent show of “The Great Night Show”, a very popular television program in the 80s."
                        :audio="require('@/assets/curso/audios/tema1/1.mp3')"
                        @audio-hover="mostrarIndicadorTarjetaAudio = false"
                        style='background-color: #fff0b5; border: 0px'
                      )
                    div
                      p.text-center.fw-bold #[em Thematic Dialogue]  / Diálogo Temático
                      TarjetaAudio.no-input.mb-3(
                        texto="Well, Pedro, one of the strangest and most exciting things I’ve experienced was when I almost won the lottery… all the numbers on the ticket came out, except for the last one. My heart nearly jumped out of my chest!"
                        :audio="require('@/assets/curso/audios/tema1/1.mp3')"
                        @audio-hover="mostrarIndicadorTarjetaAudio = false"
                        style='background-color: #fff0b5; border: 0px'
                      )
                      TarjetaAudio.no-input.mb-3(
                        texto="I can imagine!"
                        :audio="require('@/assets/curso/audios/tema1/1.mp3')"
                        @audio-hover="mostrarIndicadorTarjetaAudio = false"
                        style='background-color: #cad3f2; border: 0px'
                      )
              .col-lg-4.col-8(data-aos="fade-left"): img(src='@/assets/curso/temas/tema1/3.svg', alt='' )
      .contenedor-slyder.mb-5
        .row.justify-content-end.mb-5
          .col-lg-10
            .tarjeta.bg-white.p-5
              .row.justify-content-end.mb-5
                .col-lg-11
                  p 
                    span.r--3.fw-normal #[em Next, we are going to learn vocabulary related to some expressions used to talk about feelings, going on a trip, or life experiences.] 
                    span.r--g / A continuación, vamos a aprender vocabulario relacionado con algunas expresiones utilizadas para hablar de sentimientos, salir de viaje, o experiencias de vida.
                  SlyderF.mb-5(columnas="col-lg-6 col-xl-4")
                    .bg-sf.d-flex.align-items-end.justify-content-center.p-2(:style="{'background-image':`url(${require('@/assets/curso/temas/tema1/5.jpg')})`}")(style='height: 348px')
                      .tarjeta.bg-white.p-2.d-flex.justify-content-center.flex-column
                        Audio.color-acento-botones.d-block(:audio="require('@/assets/curso/audios/tema1/1.mp3')").m-auto.mb-2
                        p.text-center 
                          span.r--4.fw-bold Win the lottery
                          br
                          | Ganar la lotería
                    .bg-sf.d-flex.align-items-end.justify-content-center.p-2(:style="{'background-image':`url(${require('@/assets/curso/temas/tema1/6.jpg')})`}")(style='height: 348px')
                      .tarjeta.bg-white.p-2.d-flex.justify-content-center.flex-column
                        Audio.color-acento-botones.d-block(:audio="require('@/assets/curso/audios/tema1/1.mp3')").m-auto.mb-2
                        p.text-center 
                          span.r--4.fw-bold Be on T.V. 
                          br
                          | Estar o aparecer en televisión
                    .bg-sf.d-flex.align-items-end.justify-content-center.p-2(:style="{'background-image':`url(${require('@/assets/curso/temas/tema1/7.jpg')})`}")(style='height: 348px')
                      .tarjeta.bg-white.p-2.d-flex.justify-content-center.flex-column
                        Audio.color-acento-botones.d-block(:audio="require('@/assets/curso/audios/tema1/1.mp3')").m-auto.mb-2
                        p.text-center 
                          span.r--4.fw-bold Live abroad 
                          br
                          | Vivir en el exterior
                    .bg-sf.d-flex.align-items-end.justify-content-center.p-2(:style="{'background-image':`url(${require('@/assets/curso/temas/tema1/8.jpg')})`}")(style='height: 348px')
                      .tarjeta.bg-white.p-2.d-flex.justify-content-center.flex-column
                        Audio.color-acento-botones.d-block(:audio="require('@/assets/curso/audios/tema1/1.mp3')").m-auto.mb-2
                        p.text-center 
                          span.r--4.fw-bold Fall in love
                          br
                          | Enamorarse
                    .bg-sf.d-flex.align-items-end.justify-content-center.p-2(:style="{'background-image':`url(${require('@/assets/curso/temas/tema1/9.jpg')})`}")(style='height: 348px')
                      .tarjeta.bg-white.p-2.d-flex.justify-content-center.flex-column
                        Audio.color-acento-botones.d-block(:audio="require('@/assets/curso/audios/tema1/1.mp3')").m-auto.mb-2
                        p.text-center 
                          span.r--4.fw-bold Break a bone
                          br
                          | Romperse un hueso
                    .bg-sf.d-flex.align-items-end.justify-content-center.p-2(:style="{'background-image':`url(${require('@/assets/curso/temas/tema1/10.jpg')})`}")(style='height: 348px')
                      .tarjeta.bg-white.p-2.d-flex.justify-content-center.flex-column
                        Audio.color-acento-botones.d-block(:audio="require('@/assets/curso/audios/tema1/1.mp3')").m-auto.mb-2
                        p.text-center 
                          span.r--4.fw-bold Have an accident
                          br
                          | Tener un accidente
                    .bg-sf.d-flex.align-items-end.justify-content-center.p-2(:style="{'background-image':`url(${require('@/assets/curso/temas/tema1/11.jpg')})`}")(style='height: 348px')
                      .tarjeta.bg-white.p-2.d-flex.justify-content-center.flex-column
                        Audio.color-acento-botones.d-block(:audio="require('@/assets/curso/audios/tema1/1.mp3')").m-auto.mb-2
                        p.text-center 
                          span.r--4.fw-bold Sing in public 
                          br
                          |  Cantar en público
                    .bg-sf.d-flex.align-items-end.justify-content-center.p-2(:style="{'background-image':`url(${require('@/assets/curso/temas/tema1/12.jpg')})`}")(style='height: 348px')
                      .tarjeta.bg-white.p-2.d-flex.justify-content-center.flex-column
                        Audio.color-acento-botones.d-block(:audio="require('@/assets/curso/audios/tema1/1.mp3')").m-auto.mb-2
                        p.text-center 
                          span.r--4.fw-bold Get married 
                          br
                          |  Casarse
                    .bg-sf.d-flex.align-items-end.justify-content-center.p-2(:style="{'background-image':`url(${require('@/assets/curso/temas/tema1/13.jpg')})`}")(style='height: 348px')
                      .tarjeta.bg-white.p-2.d-flex.justify-content-center.flex-column
                        Audio.color-acento-botones.d-block(:audio="require('@/assets/curso/audios/tema1/1.mp3')").m-auto.mb-2
                        p.text-center 
                          span.r--4.fw-bold Experience an earthquake 
                          br
                          | Experimentar un terremoto
                    .bg-sf.d-flex.align-items-end.justify-content-center.p-2(:style="{'background-image':`url(${require('@/assets/curso/temas/tema1/14.jpg')})`}")(style='height: 348px')
                      .tarjeta.bg-white.p-2.d-flex.justify-content-center.flex-column
                        Audio.color-acento-botones.d-block(:audio="require('@/assets/curso/audios/tema1/1.mp3')").m-auto.mb-2
                        p.text-center 
                          span.r--4.fw-bold Do volunteer work 
                          br
                          | Hacer trabajo voluntario
                    .bg-sf.d-flex.align-items-end.justify-content-center.p-2(:style="{'background-image':`url(${require('@/assets/curso/temas/tema1/15.jpg')})`}")(style='height: 348px')
                      .tarjeta.bg-white.p-2.d-flex.justify-content-center.flex-column
                        Audio.color-acento-botones.d-block(:audio="require('@/assets/curso/audios/tema1/1.mp3')").m-auto.mb-2
                        p.text-center 
                          span.r--4.fw-bold Lose a loved one
                          br
                          | Perder un ser querido
                    .bg-sf.d-flex.align-items-end.justify-content-center.p-2(:style="{'background-image':`url(${require('@/assets/curso/temas/tema1/16.jpg')})`}")(style='height: 348px')
                      .tarjeta.bg-white.p-2.d-flex.justify-content-center.flex-column
                        Audio.color-acento-botones.d-block(:audio="require('@/assets/curso/audios/tema1/1.mp3')").m-auto.mb-2
                        p.text-center 
                          span.r--4.fw-bold Have a surgery
                          br
                          | Tener o someterse a una cirugía
                  .contenedor-slyder__img.d-none.d-lg-block: img(src='@/assets/curso/temas/tema1/4.png', alt='' )
    p.mb-5(data-aos='fade-right') Now it’s your turn to use the new vocabulary. Complete the following dialogue. / Ahora es su turno de usar el nuevo vocabulario. Complete el siguiente diálogo.  
    Dialogo.color-acento-contenido(:dialogo="dialogo")
      template(#nombre-actividad) Arrastrar y Soltar
      template(#titulo-actividad) #[em Practice dialogue] / Diálogo de práctica
      template(#descripcion-actividad) Arrastra y suelta cada una de las palabras en el orden correcto.  
          
      
</template>

<script>
export default {
  name: 'Tema1',
  components: {},
  data: () => ({
    ocultarEsp: true,
    ocultarEsp2: true,
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
            'Now tell me, ¿what *** been the most memorable day of your life?',
          textoEsp: 'Yo necesito el libro de biologia y las diapositivas.',
          audio: require('@/assets/curso/audios/tema1/1.mp3'),
          palabra: 'has',
        },
        {
          personaje: 'Pedro',
          textoIng:
            'My life hasn’t been as exciting as yours, but I think that the most memorable day of my life was when I *** married to my wife.',
          textoEsp: '',
          audio: require('@/assets/curso/audios/tema1/1.mp3'),
          palabra: 'got',
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

<style lang="sass">
.contenedor-slyder
  position: relative
  &__img
    width: 295px
    position: absolute
    bottom: 0
    left: 0
.bg-sf
  background-repeat: no-repeat
  background-size: cover
  background-position: center
.bg-tema1
  background-image: url('../assets/curso/temas/tema1/bg-tema1.svg')
  background-repeat: no-repeat
  background-size: cover
  background-position: center
</style>
