<script>
import AppHeader from "./components/AppHeader.vue";
import AppSearch from "./components/AppSearch.vue";
import AppCounter from "./components/AppCounter.vue";
import CardList from "./components/CardList.vue";
import axios from "axios";
import { store } from "./store";

export default {
  data() {
    return {
      store,
    };
  },
  components: {
    AppHeader,
    AppSearch,
    AppCounter,
    CardList,
  },
  created() {
    axios
      .get("https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0")
      .then((response) => (this.store.cardList = response.data.data));
  },
};
</script>

<template>
  <AppHeader />
  <main>
    <AppSearch />
    <AppCounter />
    <CardList />
  </main>
</template>

<style lang="scss">
@use "./assets/styles/general.scss" as *;

main {
  padding: 1.5rem;
  background-color: darkcyan;
}
</style>
