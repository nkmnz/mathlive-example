<template>
  <div id="app">
    $$e^{i\pi} + 1 = 0$$
    <!--
    <MathLiveComponent></MathLiveComponent>
    -->
    <ML2Tex></ML2Tex>
  </div>
</template>

<script>
import MathLive from "mathlive";
//import MathLiveComponent from "./components/MathLiveComponent.vue";
import ML2Tex from "./components/ML2Tex.vue";

export default {
  name: "app",
  components: {
    //MathLiveComponent,
    ML2Tex
  },
  data() {
    return {};
  },
  mounted: function() {
    MathLive.renderMathInDocument();
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
