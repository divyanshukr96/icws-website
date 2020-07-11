<template>
  <div class="service-container">
    <div class="backdrop"></div>
    <div class="service-container-content">
      <service-card></service-card>
      <service-card></service-card>
      <service-card></service-card>
      <service-card></service-card>
      <service-card></service-card>
    </div>
  </div>
</template>

<script>
  import ServiceCard from "./service-card";

  export default {
    name: "service-page",
    components: {ServiceCard}
  }
</script>

<style scoped>
  .service-container {
    background-color: #2B2D42;
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    text-align: center;
    position: relative;

    align-items: center;
    justify-content: center;

  }


  .service-container .backdrop {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 50%;
    background-color: #FAA916;
    margin: auto;
    z-index: 1;
  }

  .service-container-content {
    display: flex;
    max-width: 1400px;
  }


  @media only screen and (min-width: 1200px) {
    .service-container-content > div:nth-child(odd) {
      transform: translateY(-25%);
    }

    .service-container-content > div:nth-child(even) {
      transform: translateY(25%);
    }
  }

  @media only screen and (max-width: 1200px) {

    .service-container-content {
      flex-wrap: wrap;
      justify-content: center;
    }

  }

</style>
