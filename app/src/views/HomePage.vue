<template>
  <main>
    <h2>TESTERAADASD</h2>
  </main>
</template>

<script setup>
import { computed } from "vue";

const teste = "abcd";

const testMethod = (prop1, prop2) => {
  switch (prop1) {
    case "teste1":
      console.log("aaaa");
      break;
    case "teste2":
      console.log("bbbb");
      break;
    default:
      console.log("testMethod");
      break;
  }
};
//create a computed
const testComputed = computed(() => {
  return "computed value";
});
</script>
