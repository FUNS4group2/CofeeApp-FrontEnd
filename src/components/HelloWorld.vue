<template>
<!--npm install vue-slider-component!-->
<div >
     <select v-model="selected">
  <option disabled value="">Please select one</option>
  <option>Coffee</option>
  <option>Hot-Water</option>
  <option>Cappucino</option>
  </select>
<span>Selected: {{ selected }}</span>



  <h2>sugarAmount</h2>
    <vue-slider v-model="sugarAmount"></vue-slider>
  <h2> milkAmount </h2> 
    <vue-slider v-model="milkAmount"></vue-slider>
<div id="example-2">
  <!-- `greet` is the name of a method defined below -->
  <button v-on:click="greet">Greet</button>
</div>
</div>
</template>





<script>
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


<style>
#sliders {
  width : 30px;
  height: 12px;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
