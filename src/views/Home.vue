<template>
  <div class="home">
    <CalculatorContainer title="Calculator "/>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import CalculatorContainer from '@/components/CalculatorContainer.vue'; // @ is an alias to /src

export default defineComponent({
  name: 'Home',
  components: {
    CalculatorContainer,
  },
});
</script>
