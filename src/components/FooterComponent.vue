<template>
  <div class="backg vh-100"></div>
</template>

<script>
export default {
  name: "FooterComponent",
};
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables.scss" as *;
@use "../assets/styles/general.scss" as *;
.backg {
  background-image: url("img/footer-3.jpg");
  background-size: cover;
}
</style>
