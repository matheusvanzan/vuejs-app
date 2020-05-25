<template>
  <div id="app">
    <h3>Teste Vue.js</h3>
    <p>{{ msg }}</p>
    <br>
    <button @click="mudarMsg">Mudar mensagem</button>
    
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component
export default class App extends Vue {
  
  msg = 'Essa é uma mensagem carregada inicialmente'
  
  mudarMsg() {
    this.msg = 'Essa é outra mensagem carregada pelo botão'
  }
  
}
</script>

<style scoped lang="scss">
#app h3 {
  width: 100px;
  border-bottom: 1px solid gray;
}

#app button {
  background-color: white;
  width: 100px;
  border: 1px solid black;
  border-radius: 5px;
}
</style>