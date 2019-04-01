<template>
  <div id="app">
    <HelloWorld/>
    <Division/>
    <Galeria/>
    <Conctact/>
    <Footer/>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import Icons from "./components/Icons";
import Footer from "./components/Footer";
import Galeria from "./components/Galeria";
import Conctact from "./components/Conctact";
import Division from "./components/Division";

export default {
  name: "App",
  components: {
    HelloWorld,
    Icons,
    Footer,
    Galeria,
    Conctact,
    Division
  }
};
</script>

<style>
</style>
