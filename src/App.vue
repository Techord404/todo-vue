<template>
  <div class="name">
    {{ name }}
  </div>
  <input type="text" v-bind:value="name">
  <button class="btn btn-primary" v-on:click="updateName">Click</button>
</template>

<script>

import { ref } from "vue";

export default {
  setup() {
    const name = ref('Techord123');
    //
    // const greeting = (name) => {
    //   return 'Hello, ' + name;
    // };
    //
    // const greet = greeting(name);

    const updateName = () => {
      name.value = 'Techrod';
    }

    return {
      name,
      updateName
    };
  }
}
</script>

<style>
  .name {
    color: red;
  }
</style>