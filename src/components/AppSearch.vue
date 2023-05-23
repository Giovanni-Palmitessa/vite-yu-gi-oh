<script>
import { store } from "../store";
export default {
  data() {
    return {
      store,
    };
  },
  methods: {
    emitSearchEvent() {
      this.$emit("performSearch");
    },
  },
};
</script>
<template>
  <div class="container-small">
    <select
      v-model="store.searchArchetype"
      @change="emitSearchEvent"
      name="species"
      id="species"
    >
      <option value="">Seleziona Archetype</option>
      <option value="alien">Alien</option>
    </select>
  </div>
</template>

<style lang="scss" scoped></style>
