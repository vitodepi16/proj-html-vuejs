<template>
  <div class="col-sm-12 col-lg-3 col-md-6 mt-3 mx-auto">
    <div class="card text-bg-dark">
      <img :src="item.img" class="card-image h-100" alt="..." />
      <div
        class="card-img-overlay d-flex flex-column justify-content-end text-center p-0"
      >
        <h5 class="card-title">{{ item.title }}</h5>
        <p class="card-text">
          {{ item.text }}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Cardbook",
  props: ["item"],
};
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables.scss" as *;

.card {
  background-color: white;
  height: 100%;
  border-radius: 0% 0% 20% 0%;
  overflow: hidden;
  transition: all 300ms;
}
.card:hover {
  transform: translateY(-6px);
  box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25), 0 10px 10px rgba(0, 0, 0, 0.22);
  cursor: pointer;
}

.card-text {
  color: $orange-title;
}
</style>
