<template>
  <div id="app-2">
    <span v-bind:title="message">
      Hover your mouse over me for a few seconds to see my dynamically bound
      title!
    </span>
  </div>
</template>

<script setup>
import { ref } from "vue";

const message = ref("You loaded this page on " + new Date().toLocaleString());
</script>
<script setup>
// import HelloWorld from './components/HelloWorld.vue'
</script>
