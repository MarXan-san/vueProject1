<script  lang="ts">

import Component1 from "@/components/Component1/Component1.vue";
import {defineComponent} from "vue";

export default defineComponent({
  components: {Component1},
  data() {
    return {
      names: ["Maria", "Marios", "Attila", "Simeon", "Ioannis"],
      people1: [
        {
          name: "Odett",
          color: "blue"
        },
        {
          name: "David",
          color: "#f0f"
        },
        {
          name: "Daniel",
          color: "black"
        }
      ],
      people2: [
        {
          name: "Filippos",
          color: "green"
        },
        {
          name: "Ioanna",
          color: "red"
        },
        {
          name: "Adam",
          color: "orange"
        }
      ]
    }
  }
})

</script>

<template>

<Component1 :people="people1"></Component1>
  <Component1 :people="people2"></Component1>


</template>

<style scoped>

</style>
