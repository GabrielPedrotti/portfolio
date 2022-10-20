<template>
  <RouterView />
</template>

<script setup>
import { computed } from "vue";

const teste = 'abcd'

const testMethod = (prop1, prop2) => {
  console.log('testMethod')
}
//create a computed
const testComputed = computed(() => {
  return 'computed value'
})

</script>
