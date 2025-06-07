<script setup>
  import { ref, computed } from 'vue';
  const count = ref(0);
  const increment = () =>{
    if (count.value<10) count.value++
  }
  const decrement = () =>{
    if (count.value>0) count.value--
  }
  const squared = computed(()=>{
    return count.value**2;
  })
  let username = ref('')
  let friends = ref(['Me','You','Him','Her'])
  const changeUser = () => username.value = 'Pratyush'
  const removeUser = () => username.value = ''
</script>

<template>
  <h1>Count : {{ count }}</h1>
  <h1>Count squared: {{ squared }}</h1>
  <button @click="increment">Increment</button>
  <button @click="decrement">Decrement</button>
  <h1>Users: {{ username }}</h1>
  <button @click="changeUser">Add User</button>
  <button @click="removeUser">Remove User</button>
  <h1>1. {{ friends[0] }}</h1>
  <h1>2. {{ friends[1] }}</h1>
  <h1>3. {{ friends[2] }}</h1>
  <h1>4. {{ friends[3] }}</h1>
  <button @click="friends[0]='🤝'">Handshake 1</button>
  <button @click="friends[1]='🤝'">Handshake 2</button>
  <button @click="friends[2]='🤝'">Handshake 3</button>
  <button @click="friends[3]='🤝'">Handshake 4</button>
</template>
