<template>
  <div class="container text-center">
    <h2 class="fs-1 p-4 fw-bold">Dig A Little Deeper Into Damon Vaughn</h2>
    <h3 class="fs-5 p-3">FIND OUT MORE ABOUT THE AUTHOR HIMSELF</h3>
    <div class="card-book d-flex">
      <div class="row p-3 ms-4 me-4 mb-5">
        <Cardbook v-for="item in event" :item="item" />
      </div>
    </div>
  </div>
</template>

<script>
import Cardbook from "./Cardbook.vue";

export default {
  name: "PersonalBook",
  data() {
    return {
      event: [
        {
          img: "img/book-17.jpeg",
          title: "Chicago Book Signing",
          text: "Vestibulum ante ipsum primis",
        },
        {
          img: "img/book-19.jpeg",
          title: "Meet & Greet With Amanda",
          text: "Vestibulum ante ipsum primis",
        },
        {
          img: "img/book-20.jpeg",
          title: "Open Book: Dialogues",
          text: "Vestibulum ante ipsum primis",
        },
      ],
    };
  },
  components: { Cardbook },
};
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables.scss" as *;
@use "../assets/styles/general.scss" as *;
h3 {
  color: $btn-green;
}
</style>
