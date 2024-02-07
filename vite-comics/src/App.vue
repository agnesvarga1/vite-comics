<script>
import AppHeader from "./components/AppHeader.vue";
import ListDC from "./components/ListDC.vue";
import Cards from "./components/Cards.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    ListDC,
    Cards,
    AppFooter,
  },
};
</script>

<template>
  <AppHeader />
  <main>
    <ListDC />
    <Cards />
  </main>
  <AppFooter />
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
