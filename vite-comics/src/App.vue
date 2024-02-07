<script>
import AppHeader from "./components/AppHeader.vue";

import ListDC from "./components/ListDC.vue";

import Cards from "./components/Cards.vue";
export default {
  name: "App",
  components: {
    AppHeader,
    ListDC,
    Cards,
  },
};
</script>

<template>
  <AppHeader />
  <main>
    <ListDC />
    <Cards />
  </main>
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
