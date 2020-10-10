<template>
  <div class="calculator-container">
    <input class="display"/>
    <CalculatorButtons />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import CalculatorButtons from '@/components/CalculatorButtons.vue'; // @ is an alias to /src

export default defineComponent({
  name: 'Calculator',
  components: {
    CalculatorButtons,
  },
  props: {
    title: String,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .calculator-container {
  background-color: gray;
  height: 400px;
  width: 60vmax;
  margin: auto;
}
  .display {
  margin-top: 10px;
  background-color: black;
  width: 50vmax;
  height: 3em;
  color: white;
  font-weight: bold;
}
</style>
