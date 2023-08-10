<template>
  <div class="home">
    <button @click="createNewPost">New Post</button>
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  },
  methods: {
    createNewPost() {
      // Code, um einen neuen Beitrag zu erstellen oder zur Beitragserstellungsseite zu navigieren
      console.log('New Post Button was clicked!');
      alert('Klappt')
    }
}
}
</script>
<style>
.home button {
  position:absolute;
  top: 201px;
  left: 10px;
  padding: 10px 15px;
  background-color: #d3e2db; /* Farbe des Links */
  color: black;
  border: none;
  border-radius: 3px;
  cursor: pointer;
}

.home button:hover {
  background-color: #ed8e00; /* Dunklere Farbe beim Überfahren */
}

</style>
