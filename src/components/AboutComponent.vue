<template>
  <div class="container text-center p-5">
    <h1 class="p-3 fs-1">More About Demon Vaught</h1>
    <p class="p-4 lh-lg">
      Damon Vaughn is a professor of psychology at the University of Toronto, a
      clinical psychologist and the author of the multi-million copy bestseller
      “The story of my life.”
    </p>
    <button class="btn btn-lg">Meet The Author</button>
  </div>
  <div class="audiobook">
    <div class="container">
      <ul class="d-flex justify-content-center p-3">
        <li>
          <img src="img/ebay-logotan-2x-600x197.png" alt="" srcset="" />
        </li>
        <li>
          <img src="img/audible-logotan-2x-200x66.png" alt="" srcset="" />
        </li>
        <li>
          <img src="img/bb-logotan-2x.png" alt="" srcset="" />
        </li>
        <li>
          <img src="img/kindlefire-logotan-2x-200x66.png" alt="" srcset="" />
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutComponent",
};
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables.scss" as *;

.container {
  h1 {
    color: $orange-title;
    font-weight: bolder;
  }
  p {
    color: $bg-black;
    font-size: 2rem;
    line-height: 2rem;
  }

  .btn {
    background-color: $btn-green;
    font-size: small;
    color: white;
  }
  .btn:hover {
    background-color: #367d64;
    color: white;
  }

  ul {
    list-style: none;
    margin-bottom: 0;
    li {
      width: 200px;
      margin-left: 2.5rem;
      img {
        width: 100%;
      }
    }
  }
}
.audiobook {
  background-color: #fef7e9;
}
</style>
