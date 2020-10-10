<template>
  <div class="hello">
    <h1>{{ title }}</h1>
    <Calculator />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Calculator from '@/components/Calculator.vue'; // @ is an alias to /src

export default defineComponent({
  name: 'CalculatorContainer',
  props: {
    title: String,
  },
  components: {
    Calculator,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h3 {
    margin: 40px 0 0;
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #42b983;
  }
</style>
