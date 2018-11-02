<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
      <body>
        <form ref='uploadForm' 
          id='uploadForm' 
          action='http://localhost:3000/api/image/upload' 
          method='post' 
          encType="multipart/form-data">
            <input type="file" name="sampleFile" />
            <input type='submit' value='Upload!' />
        </form>     
      </body>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <GoogleMap/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import GoogleMap from './components/GoogleMaps.vue'

export default {
  name: 'app',
  components: {
    // HelloWorld
    GoogleMap
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
