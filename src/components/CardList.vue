<script>
import Card from "./Card.vue";
import { store } from "../store";

export default {
  data() {
    return {
      store,
    };
  },
  components: {
    Card,
  },
};
</script>

<template>
  <div class="container-small">
    <div class="card-list">
      <Card />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card-list {
  display: flex;
  flex-wrap: wrap;
}
</style>
