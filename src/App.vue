<script setup>
  import One from './components/One.vue';
  import ConditionalRendering from './components/ConditionalRendering.vue';
  import VFor from './components/V-for.vue';
  import Vmodel from './components/V-model.vue';
import Props from './components/Props.vue';
const name = 'some name'
const age = 40
</script>

<template>
  <One/><hr/>
  <ConditionalRendering/><hr/>
  <VFor/><hr/>
  <Vmodel/><hr/>
  <Props :name = 'name' :age = 'age'/><hr>
</template>