<template>
  <div class="backgr d-flex justify-content-center">
    <div class="box">
      <div class="text-center p-5 newsletter">
        <h1 class="p-3">Subscribe To My Newsletter</h1>
        <h3 class="p-3 fs-5">BE NOTIFIED ABOUT BOOK SIGNING TOUR DATES</h3>
        <input type="email" placeholder="Insert your email ..*" />
        <button class="btn ms-4 btn-lg">Subscribe</button>
        <p class="p-3 fs-6">
          Donec fringilla nunc eu turpis dignissim, at euismod sapien tincidunt.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "NewsletterComponent",
};
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables.scss" as *;

.backgr {
  background-image: url("img/banner-2.jpg");
  background-repeat: no-repeat;
}
.newsletter {
  padding: 8rem;
}
h1 {
  color: white;
}
h3 {
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
</style>
