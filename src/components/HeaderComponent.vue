<template>
  <div class="jumbotron">
    <div class="navbar d-flex justify-content-between align-items-center">
      <div class="nav left">
        <div class="logo ms-5">
          <img src="../../public/img/author-logo-round-small.png" alt="" />
        </div>
      </div>

      <div
        class="nav-right justify-content-center align-items-center flex-wrap d-none d-md-flex"
      >
        <ul class="d-flex flex-wrap">
          <li>Home</li>
          <li>About Me</li>
          <li>Testimonials</li>
          <li>My Blog</li>
          <li>Meetups</li>
          <li>Shop</li>
          <li>Contact Me</li>
          <li><i class="fa-solid fa-cart-shopping"></i></li>
        </ul>
      </div>
    </div>
    <div class="d-flex align-item-center justify-content-between mt-5">
      <div class="zone-title">
        <h1>Damon Vaugh</h1>
        <h2>
          Best-Selling Author And The Most Influential Public Intellectual In
          The Western World Right Now.
        </h2>
        <p>-The New York Times</p>
      </div>
      <div class="book-release p-4">
        <div class="d-flex">
          <div class="book-img">
            <img src="../../public/img/book-widget.png" class="ms-4" alt="" />
          </div>
          <div class="p-4">
            <h2>Latest Book Release</h2>
            <h3>D. VAUGHN AUTOBIOGRAPHY</h3>
            <p>
              Donec fringilla nunc eu turpis dignissim, at euismod sapien
              tincidunt. Maecenas eleifend congue cursus.
            </p>
          </div>
        </div>
        <div class="zone-btn d-flex justify-content-around p-4">
          <button class="btn btn-lg">
            <i class="fa-brands fa-amazon"></i> Buy on Amazon
          </button>
          <button class="btn btn-lg">
            <i class="fa-solid fa-apple-whole"></i> Buy on App Store
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderComponent",
};
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables.scss" as *;

ul {
  list-style: none;
  li {
    margin: 1.2rem;
    color: white;
    padding: 0.7rem;

    &:hover {
      color: $orange-title;
      cursor: pointer;
      transition: 100ms;
      border-top: solid;

      border-top-color: #f4b429;
    }
  }
}
.jumbotron {
  background-image: url("../../public/img/footer-3.jpg");
  font-weight: 800;
  h1 {
    color: $orange-title;
    font-weight: 800;
  }
  h2 {
    color: white;
    line-height: 3rem;
    font-weight: 800;
  }
  p {
    color: $bg-subtitle;
  }
  .zone-title {
    width: 40%;
    line-height: 3rem;
    margin-left: 4rem;
    margin-top: 5rem;
  }
  .book-release {
    width: 40%;
    background-color: white;
    margin-top: 10%;

    h2 {
      color: black;
      font-size: 1.5em;
    }
    h3 {
      color: $orange-title;
      font-size: medium;
      letter-spacing: 0.09em;
    }
    p {
      color: $bg-black;
    }
  }
  .zone-btn {
    .btn {
      background-color: $bg-secondary;
      border: 1px solid #49a987;
      font-size: small;
      width: 120px;
      width: fit-content;
      height: fit-content;
    }
    .btn:hover {
      background-color: #49a987;
      color: white;
    }
  }
}
.book-img {
  width: fit-content;
  img {
    width: 100%;
  }
}
.logo {
  width: 100px;
  img {
    width: 100%;
  }
}
</style>
