<template>
  <div class="backg">
    <div class="container p-5 mb-4">
      <div class="zone-up d-flex justify-content-between p-3 mt-2">
        <div class="title">
          <h1>Recent articles</h1>
          <h4 class="text-uppercase">Read the latest entries</h4>
        </div>
        <div>
          <button class="btn btn-lg mt-5">All Articles</button>
        </div>
      </div>
      <div class="zone-articles d-flex">
        <div class="zone-left">
          <div class="card mb-3">
            <div class="card-image">
              <img
                src="img/20-Tips-600x353.jpg"
                class="card-img-top"
                alt="..."
              />
              <div class="gradient"></div>
            </div>

            <div class="card-body">
              <h3 class="card-title p-1">20 Creativity Tips</h3>
              <h6 class="card-title p-1">
                By admin | October 24th, 2019 | Categories: Event, Tips & Tricks
              </h6>
              <p class="card-text lh-lg">
                Vestibulum ante ipsum primis in faucibus orci luctus et ultrices
                posuere cubilia Curae; Donec velit neque, auctor sit amet
                aliquam vel, ullamcorper sit amet.
              </p>
            </div>
          </div>
        </div>
        <div class="zone-right d-flex flex-column mx-auto">
          <div class="card mb-3">
            <img
              src="img/thumb-13-2x-320x202.jpg"
              class="card-img-top"
              alt="..."
            />
            <div class="card-body d-flex flex-column justify-content-end">
              <h3 class="card-title fw-light">What's On Your booklist</h3>
              <h6 class="card-text">
                by admin <span class="fusion-inline-sep">|</span> October 24th,
                2019
              </h6>
            </div>
          </div>
          <div class="card mb-3">
            <img
              src="img/thumb-08-2x-320x202.jpg"
              class="card-img-top"
              alt="..."
            />
            <div class="card-body d-flex flex-column justify-content-end">
              <h3 class="card-title fs-3 fw-light">Istanbul Travel Guide</h3>
              <h6 class="card-text">
                by admin <span class="fusion-inline-sep">|</span> October 24th,
                2019
              </h6>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "RecentComponent",
};
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables.scss" as *;

.backg {
  background-color: #fef7e9;
  padding: 20px;
  h4 {
    color: $btn-green;
  }

  .btn {
    background-color: $orange-title;
    color: white;
  }
  .btn:hover {
    background-color: #ca9624;
    color: white;
  }
}
.zone-left {
  width: 50%;
  .card-image {
    position: relative;
    img {
      height: 100%;
      width: 100%;
    }
    &:hover {
      cursor: pointer;
      transition: 5000ms;
      .gradient {
        display: block;
      }
    }
    .gradient {
      display: none;
      position: absolute;
      content: "";
      height: 100%;
      width: 100%;
      top: 0;
      left: 0;
      background: $bg-gradient;
    }
  }
}
.zone-right {
  width: 40%;
  .card {
    padding-bottom: 0;
    padding-top: 60%;
  }

  .card-body,
  .card-text {
    width: 100%;
    height: 100%;
    overflow: hidden;
    cursor: pointer;
    position: relative;
    margin-bottom: 0;
    text-align: center;
  }
  img {
    width: 100%;
    height: 100%;
    position: absolute;
    object-fit: cover;
    top: 0;
    left: 0;
    opacity: 0.9;
    transition: opacity 0.5s ease-out;
  }
  h3 {
    position: absolute;
    transition: inset 0.3s 0.3s ease-out;
    color: black;
  }
  h6 {
    position: absolute;
    opacity: 0;
    max-width: 80%;
    transition: opacity 0.3s ease-out;
  }

  .card-body:hover h3 {
    inset: auto auto 220px 30px;
    transition: inset 0.3s ease-out;
    background-color: transparent;
  }

  .card-body:hover p {
    opacity: 1;

    transition: opacity 0.5s 0.1s ease-in;
  }
  .card-body:hover {
    background-color: transparent;
    transition: 300ms;
  }
  .card-body:hover img {
    transition: opacity 0.3s ease-in;
    opacity: 1;
  }
}

.card {
  width: 100%;
  height: 100%;
  padding: 60px;
}
.card-body {
  background-color: white;
}
.card-text {
  width: 100%;
}
h3:hover {
  color: $orange-title;
  transition: 200ms;
  cursor: pointer;
}
</style>
