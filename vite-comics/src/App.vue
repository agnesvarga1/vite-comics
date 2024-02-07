<script>
import AppHeader from "./components/AppHeader.vue";
import ListDC from "./components/ListDC.vue";
export default {
  name: "App",
  components: {
    AppHeader,
    ListDC,
  },
};
</script>

<template>
  <AppHeader />
  <main>
    <ListDC />
  </main>
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
