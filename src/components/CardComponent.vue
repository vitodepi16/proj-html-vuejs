<template>
  <div class="col">
    <div class="card">
      <div class="card-header p-0">
        <div class="card-image">
          <img :src="item.img" class="" alt="..." />
        </div>
      </div>

      <div class="card-body">
        <h5 class="card-title">{{ item.title }}</h5>
        <p class="card-text">
          This is a longer card with supporting text below as a natural lead-in
          to additional content. This content is a little bit longer.
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
}
.card-image {
  img {
    height: 100%;
    width: 100%;
  }
}
</style>
