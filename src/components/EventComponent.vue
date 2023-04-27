<template>
  <div class="backg">
    <div class="container text-center p-4">
      <h2 class="mt-3 p-5 fw-bolder">Upcoming Event</h2>
      <h3 class="mt-3">MEET THE AUTHOR IN PERSON</h3>
    </div>
    <div class="row p-3 ms-4 me-4">
      <CardComponent v-for="item in event" :item="item" class="text-center" />
    </div>
  </div>
</template>

<script>
import CardComponent from "./CardComponent.vue";

export default {
  data() {
    return {
      event: [
        {
          img: "img/event-05.jpg",
          title: "Chicago Book Signing",
          text: "Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Praesent sapien massa, convallis a pellentesque nec, egestas.",
        },
        {
          img: "img/event-04.jpg",
          title: "Meet & Greet With Amanda",
          text: "Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Praesent sapien massa, convallis a pellentesque nec, egestas.",
        },
        {
          img: "img/event-07.jpg",
          title: "Open Book: Dialogues",
          text: "Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Praesent sapien massa, convallis a pellentesque nec, egestas.",
        },
      ],
    };
  },

  name: "EventComponent",
  components: { CardComponent },
};
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables.scss" as *;
@use "../assets/styles/general.scss" as *;

.backg {
  background-color: #fef7e9;
}
h3 {
  color: $orange-title;
}
h5:hover {
  color: $orange-title;
}
</style>
