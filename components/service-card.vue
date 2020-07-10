<template>
  <div class="card">
    <img src="~/assets/images/desktop.png" alt="">
    <p class="card-title">Web Development</p>
    <p>at icws is lorem ipsum something something add more content telling about what
      web
      development is and how we do it More and more details come here.
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
    max-width: 300px;
    margin: 16px;

    background: #2B2D42 0 0 no-repeat padding-box;
    /*border: 1px solid #707070;*/
    color: #eee;
    z-index: 5;

    height: fit-content;


    -webkit-box-shadow: 2px 4px 8px 0 rgba(0, 0, 0, 0.5);
    -moz-box-shadow: 2px 4px 8px 0 rgba(0, 0, 0, 0.5);
    box-shadow: 2px 4px 8px 0 rgba(0, 0, 0, 0.5);
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
