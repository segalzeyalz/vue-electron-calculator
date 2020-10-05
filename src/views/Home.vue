<template>
  <div class="home">
    <Calculator title="Calculator "/>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Calculator from '@/components/Calculator.vue'; // @ is an alias to /src

export default defineComponent({
  name: 'Home',
  components: {
    Calculator,
  },
});
</script>
