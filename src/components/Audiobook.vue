<template>
  <div class="audiobook">
    <div class="container d-flex justify-content-center">
      <div class="phone-book">
        <img src="img/audible-app-2x-400x418.png" alt="" />
      </div>
      <div class="shop text-center">
        <h1>New AudioBook</h1>
        <h3>NO TIME TO READ? NO PROBLEM. LISTEN TO IT</h3>
        <p>
          Donec fringilla nunc eu turpis dignissim, at euismod sapien tincidunt.
          Maecenas eleifend congue cursus.
        </p>
        <button class="btn">
          <i class="fa-brands fa-amazon me-3"></i>Buy This On Audible
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Audiobook",
};
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables.scss" as *;

.phone-book {
  margin-top: 2.5rem;
  width: 30%;
  img {
    width: 100%;
  }
}
.shop {
  width: 40%;
  margin-left: 2.5rem;
  padding: 2rem;
  margin-top: 8rem;
}
.audiobook {
  background-image: url("img/bg-book-rotate.jpeg");
  background-repeat: no-repeat;
}
h1 {
  color: white;
}
h3 {
  color: $orange-title;
  line-height: 2em;
  font-size: medium;
}
p {
  color: $bg-subtitle;
  line-height: 2em;
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
</style>
