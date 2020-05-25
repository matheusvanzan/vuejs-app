<template>
  <div class="hello">
    Essa é uma mensagem: {{ msg }}
    <br>
    <button @mudarMsg>Mudar mendagem</button>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class HelloWorld extends Vue {
  @Prop() private msg!: string;
  
}
</script>

<style scoped lang="scss">
.hello {
  margin: 10px;
}
</style>
