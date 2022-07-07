<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <vue-slider v-model="value" />
    <div>
    <Slider v-model="value" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
//import { reactive, toRefs } from 'vue'
//import VueSlider from 'vue-slider-component'
import 'vue-slider-component/theme/antd.css'
import Slider from '@vueform/slider'

export default {
  name: 'App',
  components: {
    HelloWorld,
    //VueSlider
    Slider
  },
  // setup() {
  //   const data = reactive({ value: 0 })
  //   return toRefs(data)
  // }
  data() {
    return {
      value: 20
    }
  }
}
</script>

<style src="@vueform/slider/themes/default.css">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
