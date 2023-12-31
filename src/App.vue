<template>
  <div class="name">
    {{ name }}
  </div>
  <button class="btn btn-primary" v-on:click="updateName">Click</button>
</template>

<script>
export default {
  setup() {
    let name = 'Techord123';
    //
    // const greeting = (name) => {
    //   return 'Hello, ' + name;
    // };
    //
    // const greet = greeting(name);

    const updateName = () => {
      name = 'Techrod';
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