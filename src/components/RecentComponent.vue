<template>
  <div class="backg">
    <div class="container">
      <div class="zone-up d-flex justify-content-between p-3 mt-2">
        <div class="title">
          <h1>Recent articles</h1>
          <h4 class="text-uppercase">Read the latest entries</h4>
        </div>
        <div>
          <button class="btn btn-lg mt-5">All Articles</button>
        </div>
      </div>
      <div class="zone-articles">
        <div class="zone-left">
          <div class="card mb-3">
            <img src="img/20-Tips-600x353.jpg" class="card-img-top" alt="..." />
            <div class="card-body">
              <h5 class="card-title">Card title</h5>
              <p class="card-text">
                This is a wider card with supporting text below as a natural
                lead-in to additional content. This content is a little bit
                longer.
              </p>
              <p class="card-text">
                <small class="text-body-secondary"
                  >Last updated 3 mins ago</small
                >
              </p>
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
@use "../assets/styles/general.scss" as *;
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
}
.card {
  background-color: white;
  padding: 20px;
}
</style>
