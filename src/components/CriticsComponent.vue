<template>
  <div class="container">
    <h2 class="p-3 fw-bolder mt-5">What the Critics Say</h2>
    <h3 class="p-3 fw-light" style="color: #49a987">
      TESTIMONIALS FROM AROUND THE WORLD
    </h3>
    <div class="d-flex justify-content-around">
      <section class="section-left h-100">
        <div class="card card-left text-bg-dark h-100">
          <img src="img/testimonials.jpeg" class="h-100" alt="..." />
          <div class="card-img-overlay">
            <h5 class="card-title fs-1 p-3 ms-4">
              Best Author of His Generation
            </h5>
            <div class="line m-5"></div>
            <div class="text-start ms-4">
              <h2 class="card-text mt-2 mb-2 p-2 fs-3">
                This Book will change your perspective on life
              </h2>
              <p class="card-text lh-base mt-2">
                <small
                  >Donec rutrum congue leo eget malesuada. Vivamus suscipit
                  tortor eget felis porttitor volutpat. Nulla quis lorem ut
                  liber. Proin eget tortor risus. Praesent sapien massa,
                  convallis a pellentesque nec, egestas non nisi. Donec rutrum
                  congue leo eget malesuada.</small
                >
              </p>
              <p class="card-text lh-base mt-3">
                <small
                  >Donec fringilla nunc eu turpis dignissim, at euismod sapien
                  tincidunt. Maecenas eleifend congue cursus. In vitae enim quis
                  sem pharetra.Curabitur arcu erat, accumsan id imperdiet et,
                  porttitor at sem.</small
                >
              </p>
              <p class="card-text mt-5">
                <img src="img/nytimes-logo-white-xsmall.png" alt="" />
                Justine Kilpatrick,
                <span style="color: #49a987">The New York Times</span>
              </p>
            </div>
          </div>
        </div>
      </section>
      <section class="section-right">
        <button class="btn">Read All Testimonials</button>
        <div class="recens">
          <div class="card mb-3 card-recen mt-5">
            <div class="card-header fw-bolder">A True Masterpiece, Bravo!</div>
            <div class="card-body">
              <p class="card-text lh-lg p-4">
                Nulla quis lorem ut libero malesuada feugiat. Vivamus magna
                justo, lacinia eget consectetur sed, convallis at tellus.
                Vivamus suscipit tortor eget felis porttitor volutpat. Nulla
                quis lorem ut libero malesuada feug at.
              </p>
            </div>
          </div>
          <h3 class="fs-5">
            <img class="me-4" src="img/theguardian-xsmall.png" alt="" />
            Gerald Hendley, <span class="fs-6 giornalist">The Guardian </span>
          </h3>
        </div>
        <div class="recens">
          <div class="card mb-3 card-recen mt-5">
            <div class="card-header fw-bolder">A Unique View On The World</div>
            <div class="card-body">
              <p class="card-text lh-lg p-4">
                Donec sollicitudin molestie malesuada. Curabitur arcu erat,
                accumsan id imperdiet et, porttitor at sem. Vestibulum ac diam
                sit amet quam vehicula elementum sed sit amet dui. Nulla quis
                lorem ut libero malesuada feugiat. Vestibulum ac diam sit amet.
              </p>
            </div>
          </div>
          <h3 class="fs-5">
            <img class="me-4" src="img/globe-xsmall.png" alt="" />
            Mary Maxey,<span class="fs-6 giornalist">The Globe And Mail</span>
          </h3>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
export default {
  name: "CriticsComponent",
};
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables.scss" as *;

.section-left {
  width: 50%;
}
.section-right {
  width: 50%;
  .recens {
    margin-left: 20%;
    width: 80%;
  }
}
.card-recen {
  background-color: #fef7e9;
  width: 100%;
  text-align: center;
}
.giornalist {
  color: black;
  cursor: pointer;
}
.giornalist:hover {
  color: $orange-title;
  transition: 300ms;
}
.card-left {
  width: 100%;
  height: 80%;
  border-radius: 0% 0% 25% 0%;
  margin: 2rem 0rem 2rem 0rem;
  overflow: hidden;
  img {
    object-fit: cover;
  }

  .line {
    border: 0.5px solid white;
    width: 80%;
    margin: 1.4rem;
  }
  &:hover {
    transform: translateY(-10px);

    box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25), 0 10px 10px rgba(0, 0, 0, 0.22);
    cursor: pointer;
    transition: 200ms;
  }
}
.btn {
  background-color: $orange-title;
  color: white;
  margin-left: 70%;
}
.btn:hover {
  background-color: #ca9624;
  color: white;
}
</style>
