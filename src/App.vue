<<<<<<< HEAD
<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <ul>
      <li><a href="https://vuejs.org" target="_blank">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank">Forum</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank">Twitter</a></li>
    </ul>
    <h2>Ecosystem</h2>
    <ul>
      <li><a href="http://router.vuejs.org/" target="_blank">vue-router</a></li>
      <li><a href="http://vuex.vuejs.org/" target="_blank">vuex</a></li>
      <li><a href="http://vue-loader.vuejs.org/" target="_blank">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank">awesome-vue</a></li>
    </ul>
  </div>
</template>

<script>
=======
<template lang="pug">
  #app
    img(src='./assets/logo.png')
    h1 PlatziMusic
    ul
      li(v-for="artist in artists") {{artist.name}}
   
</template>

<script>
import getArtists from './api'
>>>>>>> Se realizo un request con promesas y se configuro para que salieran los nombres desde el servidor web en este caso fmmusic
export default {
  name: 'app',
  data () {
    return {
<<<<<<< HEAD
      msg: 'Welcome to Your Vue.js App'
    }
=======
      artists:[]
    }
  },
  mounted: function(){
    const self=this
    getArtists()
    .then(function (artists){
      self.artists= artists

    })
>>>>>>> Se realizo un request con promesas y se configuro para que salieran los nombres desde el servidor web en este caso fmmusic
  }
}
</script>

<<<<<<< HEAD
<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
=======
<style lang="stylus">
#app
  font-family 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing antialiased
  -moz-osx-font-smoothing grayscale
  text-align center
  color #2c3e50
  margin-top 60px

h1, h2
  font-weight normal

ul
  list-style-type none
  padding 0

li
  display inline-block
  margin 0 10px

a
  color #42b983
>>>>>>> Se realizo un request con promesas y se configuro para que salieran los nombres desde el servidor web en este caso fmmusic
</style>
