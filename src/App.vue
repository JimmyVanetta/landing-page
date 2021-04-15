<template>
  <div id="app">
    <div id="mainpic">
      <img id="peepo" alt="Happy Peepo" src="./assets/happy_peepo.png">
      <img id="leftpupil" alt="Left Pupil" src="./assets/left_pupil.png">
      <Landing msg="Welcome to my App, fren!"/>
    </div>
  </div>
</template>

<script>
import Landing from './components/Landing.vue'

export default {
  name: 'App',
  components: {
    Landing
  },
}
// JQuery //
//  ready: function() {
//  jQuery("#leftpupil").jqEye();
//  }
</script>

<style>
#app {
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#mainpic {
  display:block;
  max-height: 550px;
  margin-left: auto;
  margin-right: auto;
}
#peepo {
  z-index: 1;
  display:inline-block;
}
#leftpupil {
  z-index: -1;
  display:inline-block;
  position:relative;
  left:-397px;
  top:-256px;
}
</style>
