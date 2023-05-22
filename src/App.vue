<script>
import AppHeader from "./components/AppHeader.vue";
import AppSearch from "./components/AppSearch.vue";

export default {
  components: {
    AppHeader,
    AppSearch,
  },
};
</script>

<template>
  <AppHeader />
  <main>
    <AppSearch />
  </main>
</template>

<style lang="scss">
@use "./assets/styles/general.scss" as *;
</style>
