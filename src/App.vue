<script>
import AppHeader from "./components/AppHeader.vue";
import AppSearch from "./components/AppSearch.vue";
import AppCounter from "./components/AppCounter.vue";

export default {
  components: {
    AppHeader,
    AppSearch,
    AppCounter,
  },
};
</script>

<template>
  <AppHeader />
  <main>
    <AppSearch />
    <AppCounter />
  </main>
</template>

<style lang="scss">
@use "./assets/styles/general.scss" as *;

main {
  padding: 1.5rem;
  background-color: darkcyan;
}
</style>
