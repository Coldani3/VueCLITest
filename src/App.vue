<template>
  <DynamicList listName="TODO-List:" />
  <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
</template>

<script>
//import HelloWorld from "./components/HelloWorld.vue";
import DynamicList from "./components/VueTest.vue";

export default {
  name: "App",
  components: {
    DynamicList
  }
};
</script>