<template>
  <div id="app">
    <app-layout>
      <router-view />
    </app-layout>
  </div>
</template>

<script>
import AppLayout from "@/layouts/AppLayout.vue";

export default {
  name: "App",
  components: {
    AppLayout,
  },
  created() {
    this.$store.dispatch("init");
  },
};
</script>

<style lang="scss">
@import "~@/assets/scss/libs/normalize.scss";
@import "~@/assets/scss/fonts.scss";
@import "~@/assets/scss/scaffolding.scss";
@import "~@/assets/scss/visually-hidden.scss";
@import "~@/assets/scss/app";
</style>
