<template>
  <div class="card">
    <img src="~/assets/images/desktop.png" alt="">
    <p class="card-title">Web Development</p>
    <p>at icws is lorem ipsum something something add more content telling about what
      web
      development is and how we do it More and more details come here. Content work needs to be done still and we
    </p>
  </div>
</template>

<script>
    export default {
        name: "service-card"
    }
</script>

<style scoped>
  .card {
    padding: 20px;
    border-radius: 8px;

    background: #2B2D42 0 0 no-repeat padding-box;
    border: 1px solid #707070;
    color: #eee;
  }

  .card .card-title {
    font-size: 16px;
    color: #FFFFFF;
    margin-bottom: .5em;
  }


  .card img {
    width: 120px;
  }
</style>
