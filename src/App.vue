<template>
  <div id="app">
    <!-- Basic interpolation -->
    <span>{{msg}}</span><br>
    <!-- Using the v-text directives -->
    <span v-text="msg"></span><br>
    <!-- Parsing html -->
    <span v-html="msg"></span><br>
    <!-- Occur only once i.e. no changes reflect -->
    <span v-once>{{msg}}</span>
    <!-- If statement -->
    <p v-if="show">This is shown</p>
    <!-- Else statement -->
    <p v-else>This is not</p>
    <!-- Show statement -->
    <p v-show="show">This is Show</p>
    <!-- For loop -->
    <p v-for="user in users" v-bind:key="user.name" >{{user.name}}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
      show: true,
      users: [
        {
          name: "Surajit"
        },
        {
          name: "Laxmi"
        }
      ]
    };
  }
};
</script>


