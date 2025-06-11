<script setup>
import One from './components/One.vue';
import ConditionalRendering from './components/ConditionalRendering.vue';
import VFor from './components/V-for.vue';
import Vmodel from './components/V-model.vue';
import Props from './components/Props.vue';
import ComponentEvent from './components/ComponentEvent.vue';
import SlotComponent from './components/SlotComponent.vue';
const name = 'some name'
const age = 40
const formHandler = (username, password, email) => {
  console.log('username:', username)
  console.log('email:', email)
  console.log('password:', password)
}
</script>

<template>
  <One/><hr/>
  <ConditionalRendering/><hr/>
  <VFor/><hr/>
  <Vmodel/><hr/>
  <Props :name = 'name' :age = 'age'/><hr/>
  <ComponentEvent @UserInfo="formHandler" /> <hr/>
  <SlotComponent>
    <h1>Slot Component</h1>
    <h2>This appears between the slot tag</h2>
  </SlotComponent><hr/>
</template>