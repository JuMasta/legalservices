<template>
  <div id="app">
    <Header></Header>
    <siteContent></siteContent>
    <paySection></paySection>
    <zakon></zakon>
    <possibilities></possibilities>
    <!-- <customMap></customMap> -->
    <help></help>
    <taboo></taboo>
    <customMap></customMap>
    <chat  v-bind:messages="messages" ></chat>

  </div>
</template>

<script>

import Header from './components/New_Header.vue'
import siteContent from './components/SiteContent.vue'
import paySection from './components/pay-section.vue'
import zakon from './components/zakonadatelstvo.vue'
import possibilities from './components/possibilities.vue'
import customMap from './components/map.vue'
import taboo from './components/taboo.vue'
import help from './components/who-need-our-help.vue'
import chat from './components/Chat.vue'

export default {
  name: 'App',
  data: function()
  {
  return {
  messages: [
    
  ]
  }
  },
  components: {
    Header,
    siteContent,
    paySection,
    zakon,
    possibilities,
    customMap,
    taboo,
    help,
    chat

  }
}
</script>

<style>
*{
  box-sizing: border-box;
  text-decoration: none;
  list-style: none;
  margin:0;
  padding: 0;
}

</style>
