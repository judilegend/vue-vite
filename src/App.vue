<template>
  <div>
    <!-- Bouton avec état et texte conditionnels -->
    <button :disabled="isButtonDisabled">
      {{ isButtonDisabled ? "yes" : "non" }}
    </button>

    <!-- Bouton pour changer l'état de isButtonDisabled -->
    <button @click="toggleButtonState">Toggle Button State</button>
  </div>
</template>

<script>
import { onMounted } from "vue";

onMounted(() => {
  console.log(`the component is now mounted.`);
});
export default {
  data() {
    return {
      isButtonDisabled: true, // Initialement désactivé
    };
  },
  methods: {
    toggleButtonState() {
      // Inverse l'état de isButtonDisabled
      this.isButtonDisabled = !this.isButtonDisabled;
    },
  },
};
</script>
