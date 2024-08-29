<script setup>
// import HelloWorld from './components/HelloWorld.vue'
// import TheWelcome from './components/TheWelcome.vue'
import Nev from './components/Nev.vue'
import Card from './components/Card.vue'
import footerBT from './components/footerBT.vue'
import items from './cardDT.json'
</script>

<template>
<div>
  <header>
    <Nev />
    <h1>12 สถานที่เที่ยวประเทศไทย</h1>
    <Card v-bind="items[0]"/>
    <Card v-bind="items[1]"/>
    <Card v-bind="items[2]"/>
    <Card v-bind="items[3]"/>
    <Card v-bind="items[4]"/>
    <Card v-bind="items[5]"/>
    <Card v-bind="items[6]"/>
    <Card v-bind="items[7]"/>
    <Card v-bind="items[8]"/>
    <Card v-bind="items[9]"/>
    <Card v-bind="items[10]"/>
    <Card v-bind="items[11]"/>
  </header>

  <main>
    <!--<TheWelcome />-->
    
  </main>
  <footer>
    <footerBT />
  </footer>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Kanit&display=swap');
*{
    box-sizing: border-box;
    font-family: 'Kanit', sans-serif;
}
h1 {
  padding-top: 10px;
  padding-bottom: 10px;
  text-align: center;
}

.grid-container {
  display: grid;
  grid-column-gap: 0.5rem;
  grid-row-gap: 0.5rem;
}
@media (min-width: 576px) {
  .grid-container { grid-template-columns: repeat(1, 1fr); }
}
@media (min-width: 992px) {
  .grid-container { grid-template-columns: repeat(3, 1fr); }
}
</style>
