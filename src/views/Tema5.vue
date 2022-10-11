<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 5
      h1 #[em Exclamation phrases] (Frases de exclamación)   
    .row.justify-content-center.mb-5
      .col-lg-8(data-aos="fade-left")
        .contenedor-traductor(style='background-color: #fcf2ca').mb-5
          .contenedor-traductor__eng
            p.fst-italic  Exclamations are used to express surprise, shock, or strong emotion about something. When writing, an exclamation point (!) is usually placed at the end of the exclamatory phrase. Unlike Spanish, English doesn’t have an opening exclamation mark at the beginning of the phrase.
              br
              |Example:
              br
              br
              |I can’t believe it!
              br
              |Oh, no! Look at this place!
              br
              br
              |Next, you are invited to listen to the following thematic dialogue with exclamation phrases that are used in some English conversations.
          .contenedor-traductor__esp(:class="{ mostrar: ocultarEsp}")
            //TODO Agregar traducción
            p 
          a.boton-traduccion(@click='ocultarEsp = !ocultarEsp' style='background-color: #fc5f65') Ver traducción
      .col-lg-4.col-8(data-aos="fade-right"): img(src='@/assets/curso/temas/tema5/1.jpg', alt='' style='border-radius: 20px')
    .margin-n.p-5.mb-5.bg-tema(data-aos="zoom-in")
      h4.text-center
        span.r--2 #[em Thematic Dialogue]  / Diálogo temático
      p.mb-5(data-aos='fade-right').text-white.text-center  Dialogue between two friends, one of them had an accident at home. / Diálogo entre dos amigos, uno de ellos tuvo un accidente en casa. 
      .row.justify-content-center.mb-5
        .col-lg-9
          .tarjeta.bg-white.p-5.tarjeta-intro 
            .row.justify-content-center.mb-5
              .col-lg-6: img(src='@/assets/curso/temas/tema5/2.svg', alt='') 
              
              .col-lg-6
                TarjetaAudio.no-input.mb-3(
                    texto="<b> Kevin:</b> Manuela, I haven’t sent you my part of the group project because yesterday I broke my arm in three pieces."
                    :audio="require('@/assets/curso/audios/tema1/1.mp3')"
                    @audio-hover="mostrarIndicadorTarjetaAudio = false"
                    style='background-color: #cad3f2; border: 0px'
                  )
                TarjetaAudio.no-input.mb-3(
                    texto="<b> Manuela:</b> You can’t be serious! What happened?"
                    :audio="require('@/assets/curso/audios/tema1/1.mp3')"
                    @audio-hover="mostrarIndicadorTarjetaAudio = false"
                    style='background-color: #fff0b5; border: 0px'
                  )
            .row.justify-content-center
              
              .col-lg-6
                TarjetaAudio.no-input.mb-3(
                    texto="<b> Kevin:</b> I had an accident at home. I slipped and rolled down the stairs."
                    :audio="require('@/assets/curso/audios/tema1/1.mp3')"
                    @audio-hover="mostrarIndicadorTarjetaAudio = false"
                    style='background-color: #cad3f2; border: 0px'
                  )
                TarjetaAudio.no-input.mb-3(
                    texto="<b> Manuela:</b> Sounds awful! I hope you feel better today."
                    :audio="require('@/assets/curso/audios/tema1/1.mp3')"
                    @audio-hover="mostrarIndicadorTarjetaAudio = false"
                    style='background-color: #fff0b5; border: 0px'
                  )
              .col-lg-6: img(src='@/assets/curso/temas/tema5/3.svg', alt='') 
            .tarjeta-intro__icon1: img(src='@/assets/curso/portada/a4.svg', alt='')
            .tarjeta-intro__icon2: img(src='@/assets/curso/portada/a5.svg', alt='')
    p.mb-5(data-aos='fade-right')
      span.r--1 Let’s look at some of the most commonly used exclamatory phrases to express strong emotions in the English language: 
      span.r--g / Veamos algunas de las frases exclamativas más comúnmente usadas para expresar emociones fuertes en el idioma inglés:
    .bg-5.p-4.mb-5
      p.mb-5(data-aos='fade-right') #[em Knowing expressions or ways of expressing feelings and emotions when communicating.] / Conocer expresiones o formas de expresar los sentimientos y emociones a la hora de comunicarnos. 
      ImagenInfografica.color-acento-botones.mb-5
        template(v-slot:imagen)
          figure
            img(src='@/assets/curso/temas/tema5/4.svg', alt='Texto que describa la imagen')
        .tarjeta.p-3(x="8.5%" y="90%" numero="+" style='background-color: #f0f4ff ; border: 2px solid #89b1f3')
          h4.text-center 
          TarjetaAudio.mb-3(
            texto="<span class=' w-normal r--b' > </span>"
            :audio="require('@/assets/curso/audios/tema1/1.mp3')"
            @audio-hover="mostrarIndicadorTarjetaAudio = false"
            )
          h4
          p 
        .tarjeta.p-3(x="25%" y="90%" numero="+" style='background-color: #f0f4ff ; border: 2px solid #89b1f3')
          h4.text-center 
          TarjetaAudio.mb-3(
            texto="<span class=' w-normal r--b' > </span>"
            :audio="require('@/assets/curso/audios/tema1/1.mp3')"
            @audio-hover="mostrarIndicadorTarjetaAudio = false"
            )
          h4
          p 
        .tarjeta.p-3(x="41.5%" y="90%" numero="+" style='background-color: #f0f4ff ; border: 2px solid #89b1f3')
          h4.text-center 
          TarjetaAudio.mb-3(
            texto="<span class=' w-normal r--b' > </span>"
            :audio="require('@/assets/curso/audios/tema1/1.mp3')"
            @audio-hover="mostrarIndicadorTarjetaAudio = false"
            )
          h4
          p 
        .tarjeta.p-3(x="57.9%" y="90%" numero="+" style='background-color: #f0f4ff ; border: 2px solid #89b1f3')
          h4.text-center 
          TarjetaAudio.mb-3(
            texto="<span class=' w-normal r--b' > </span>"
            :audio="require('@/assets/curso/audios/tema1/1.mp3')"
            @audio-hover="mostrarIndicadorTarjetaAudio = false"
            )
          h4
          p 
        .tarjeta.p-3(x="74.5%" y="90%" numero="+" style='background-color: #f0f4ff ; border: 2px solid #89b1f3')
          h4.text-center 
          TarjetaAudio.mb-3(
            texto="<span class=' w-normal r--b' > </span>"
            :audio="require('@/assets/curso/audios/tema1/1.mp3')"
            @audio-hover="mostrarIndicadorTarjetaAudio = false"
            )
          h4
          p 
        .tarjeta.p-3(x="91%" y="90%" numero="+" style='background-color: #f0f4ff ; border: 2px solid #89b1f3')
          h4.text-center 
          TarjetaAudio.mb-3(
            texto="<span class=' w-normal r--b' > </span>"
            :audio="require('@/assets/curso/audios/tema1/1.mp3')"
            @audio-hover="mostrarIndicadorTarjetaAudio = false"
            )
          h4
          p 
      
          








    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    Dialogo.color-acento-contenido(:dialogo="dialogo")
      template(#nombre-actividad) Arrastrar y Soltar
      template(#titulo-actividad) #[em Seismic activity] / Actividad sísmica
      template(#descripcion-actividad)   







</template>

<script>
export default {
  name: 'Tema5',
  data: () => ({
    ocultarEsp: true,
    ocultarEsp2: true,
    ocultarEsp3: true,
    ocultarEsp4: true,
    ocultarEsp5: true,
    ocultarEsp6: true,
    dialogo: {
      personajes: [
        {
          nombre: 'Lucas',
          img: require('@/assets/curso/temas/tema3/lucas.svg'),
        },
        {
          nombre: 'Victoria',
          img: require('@/assets/curso/temas/tema3/victoria.svg'),
        },
      ],
      dialogo: [
        {
          personaje: 'Lucas',
          textoIng:
            'The moment the ground stopped shaking I knew I wanted to *** back home. I shouldn’t have moved to this city with such seismic activity.',
          textoEsp: '',
          audio: require('@/assets/curso/audios/tema1/1.mp3'),
          palabra: 'go',
        },
        {
          personaje: 'Victoria',
          textoIng: 'What a ***! You should come back.',
          textoEsp: '',
          audio: require('@/assets/curso/audios/tema1/1.mp3'),
          palabra: 'nightmare',
        },
      ],
    },
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

<style lang="sass">
.bg-5
  background-image: url('../assets/curso/temas/tema5/bg-5.png')
  background-repeat: no-repeat
  background-position: center
  background-size: 100% 100%
.bg-tema
  background-image: url('../assets/curso/temas/tema3/bg-3.svg')
  background-repeat: no-repeat
  background-position: center
  background-size: 100% 100%
.imagen-absolute
  position: relative
  margin-right: 50px
  &__img
    position: absolute
    top: 0
    right: 0
    transform: translate(50%)
</style>
