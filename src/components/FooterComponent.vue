<template>
  <div class="backg">
    <div class="row m-0 p-3">
      <div class="col mt-5">
        <div class="ms-5 logo">
          <img src="img/author-logo-round-200x205.png" alt="" />
        </div>
      </div>
      <div class="col mt-5">
        <h2>ABOUT ME</h2>
        <p class="lh-lg fw-lighter">
          Vivamus suscipit tortor eget felis porttitor volutpat. Nulla quis
          lorem ut libero malesuada feugiat. Vivamus suscipit tortor eget felis
          porttitor volutpat.
        </p>
      </div>
      <div class="col mt-5 links">
        <ul>
          <h2>USEFUL LINKS</h2>
          <li><i class="fa-solid fa-angle-right me-2"></i> latest book</li>
          <li><i class="fa-solid fa-angle-right me-2"></i> upcoming event</li>
          <li><i class="fa-solid fa-angle-right me-2"></i> recent articles</li>
          <li>
            <i class="fa-solid fa-angle-right me-2"></i> business enquires
          </li>
          <li>
            <i class="fa-solid fa-angle-right me-2"></i> visit my fundation
          </li>
        </ul>
      </div>
      <div class="col mt-5">
        <h2 class="text-uppercase">contact info</h2>
        <ul class="p-2">
          <li>63 E. Studebaker Street Bolingbrook, IL 60440</li>
          <li>Phone: (800) 000-0000</li>
          <li>Mobile: (800) 000-0000</li>
          <li>Email: <span class="hover"> info@your-company.com </span></li>
          <li>social</li>
        </ul>
      </div>
      <p class="text-center mt-5 p-3">
        © Copyright 2012 - 2023 | Avada Theme by
        <span class="hover">ThemeFusion </span> | All Rights Reserved | Powered
        by <span class="hover">WordPress </span>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterComponent",
};
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables.scss" as *;

.backg {
  background-image: url("img/footer-3.jpg");
  background-size: cover;
  color: white;
  h2 {
    font-size: medium;
  }
  .links {
    li {
      margin-top: 0.7rem;
      color: $bg-subtitle;
      &:hover {
        color: $orange-title;
        cursor: pointer;
      }
    }
  }
  .hover:hover {
    color: $orange-title;
    cursor: pointer;
  }
  p {
    color: $bg-subtitle;
    padding: 1rem;
  }
}
ul {
  list-style: none;
  li {
    margin-top: 0.7rem;
    color: $bg-subtitle;
  }
}
</style>
