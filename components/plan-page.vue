<template>
  <div class="plan-container">

    <div class="backdrop"></div>


    <plan-card></plan-card>
    <plan-card></plan-card>
    <plan-card></plan-card>

  </div>
</template>

<script>
  import PlanCard from "./plan-card";

  export default {
    name: "plan-page",
    components: {PlanCard}
  }
</script>

<style scoped>
  .plan-container {
    background-color: #FAA916 !important;
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    /*flex-direction: row-reverse;*/
    align-items: center;
    justify-content: center;
    text-align: center;
    position: relative;
  }

  .plan-container .backdrop {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 50%;
    background-color: #2B2D42;
    margin: auto;
    z-index: 1;
  }

  .plan-container > div {
    width: 350px;
    z-index: 5;
  }

</style>
