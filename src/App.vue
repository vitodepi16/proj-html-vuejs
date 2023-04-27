<template>
  <HeaderComponent />
  <AboutComponent />
  <Audiobook />
  <CriticsComponent />
  <EventComponent />
  <NewsletterComponent />
  <PersonalBook />
  <RecentComponent />
  <FooterComponent />
</template>

<script>
import AboutComponent from "./components/AboutComponent.vue";
import HeaderComponent from "./components/HeaderComponent.vue";
import Audiobook from "./components/Audiobook.vue";
import NewsletterComponent from "./components/NewsletterComponent.vue";
import CriticsComponent from "./components/CriticsComponent.vue";
import EventComponent from "./components/EventComponent.vue";
import PersonalBook from "./components/PersonalBook.vue";
import RecentComponent from "./components/RecentComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";
export default {
  name: "App",
  components: {
    HeaderComponent,
    AboutComponent,
    Audiobook,
    CriticsComponent,
    NewsletterComponent,
    EventComponent,
    PersonalBook,
    RecentComponent,
    FooterComponent,
  },
};
</script>

<style lang="scss" scoped></style>
