<template>
  <q-page class="container">
    <div class="row justify-center q-col-gutter-sm">
      <img class="col-xs-8 col-md-4" alt="Quasar logo" src="~assets/quasar-logo-full.svg">
      <q-input class="col-10" outlined disable v-model="name" label="Name" />
    </div>
    <q-page-sticky position="bottom-right" :offset="[18, 58]">
      <q-btn round color="primary" icon="keyboard_voice" size="xl" @click="enviar_voz()" />
    </q-page-sticky>
    <span>mudou dnv!</span>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
  data () {
    return {
      name: ''
    }
  },
  methods: {

    enviar_voz: function(){
      try {
        alert(window.TTS);    
      } catch (e) {
        alert(e);
      }

    }
  }
}
</script>