<template>
  <div class="home">
    <appointment/>
  </div>
</template>

<script>
// @ is an alias to /src
import Appointment from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    Appointment
  }
}


import vueSlider from 'vue-slider-component';

export default {
  components: {
    vueSlider
  },
  data () {
    return {
      value: 0
    }
  }
}


</script>