<template>
  <div class="col">
    <div class="card mb-5">
      <div class="card-header p-0">
        <div class="card-image">
          <img :src="item.img" class="" alt="..." />
        </div>
      </div>

      <div class="card-body">
        <h5 class="card-title p-4">{{ item.title }}</h5>
        <div class="line mx-auto"></div>
        <p class="card-text p-3">
          {{ item.text }}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardComponent",
  props: ["item"],
};
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables.scss" as *;
@use "../assets/styles/general.scss" as *;
.card {
  background-color: white;
  h5:hover {
    color: $orange-title;
    cursor: pointer;
    transition: 200ms;
  }
  .line {
    border: 0.5px solid $bg-subtitle;
    width: 50%;

    margin: 1.4rem;
  }
}
.card-image {
  img {
    height: 100%;
    width: 100%;
  }
}
</style>
