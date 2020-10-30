<template>
  <DynamicList listName="TODO-List:" />
</template>

<script>
import DynamicList from "./components/VueTest.vue";

export default {
  name: "App",
  components: {
    DynamicList
  }
};
</script>