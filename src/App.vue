<script setup>
import ExpandBox from './components/ExpandBox.vue';
import Card from './componentes/Card.vue'

  const caixas = [
    {id: 1, title: 'caixa 1'},
    {id: 2, title: 'caixa 2', qtde: 20},
    {id: 3, title: 'caixa 3', content: 'Conteúdo secreto da caixa 3'},
    {id: 4, title: 'caixa 4', content: 'Nubank', qtde: 5}
  ]

</script>

<template>
  <h1>Slots</h1>
  <CardFull>
    Função: estudantes
    <template #header>

  </CardFull>
  <Card>
    <h1>Ester, Juliane, Ruama</h1>
  </Card>
  <hr />
  <h1>Props</h1>
  <input type="text" v-model="titulo">
  <button></button>
  <!-- <ExpandBox title="Caixa 1" content="conteúdo 21" qtde="200000"/>
  <ExpandBox title="Caixa 2" content="conteúdo 12" qtde="35"/> -->

  <ExpandBox v-for="caixa in caixas" :key="caixa.id" v-bind="caixa" />

</template>

<style scoped>

</style>
