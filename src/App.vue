<template>
  <HeaderComponent />
  <AboutComponent />
  <Audiobook />
  <CriticsComponent />
  <NewsletterComponent />
</template>

<script>
import AboutComponent from "./components/AboutComponent.vue";
import HeaderComponent from "./components/HeaderComponent.vue";
import Audiobook from "./components/Audiobook.vue";
import NewsletterComponent from "./components/NewsletterComponent.vue";
import CriticsComponent from "./components/CriticsComponent.vue";
export default {
  name: "App",
  components: {
    HeaderComponent,
    AboutComponent,
    Audiobook,
    CriticsComponent,
    NewsletterComponent,
  },
};
</script>

<style lang="scss" scoped></style>
