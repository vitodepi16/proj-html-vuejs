<template>
  <HeaderComponent />
  <AboutComponent />
</template>

<script>
import AboutComponent from "./components/AboutComponent.vue";
import HeaderComponent from "./components/HeaderComponent.vue";
export default {
  name: "App",
  components: { HeaderComponent, AboutComponent },
};
</script>

<style lang="scss" scoped></style>
