
<script>
import {defineComponent} from "vue";

export default defineComponent({
  name: "Component1",
  props: {
    people: {
      default: 0
    }
  }

});
</script>

<template>

  <ul>
<!--    <li v-for="name in names">{{ name }}!</li>-->
    <li v-for="person in people" :style="{'color':person.color}">{{ person.name }}!</li>
  </ul>

</template>


<style scoped>

/*li:nth-child(odd){*/
/*  color: burlywood;*/
/*}*/

/*li:nth-child(even){*/
/*  color: red;*/
/*}*/

</style>