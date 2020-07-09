<template>
  <div class="plan-container">

    <div>
      <plan-card></plan-card>
    </div>

    <div>
      <plan-card></plan-card>
    </div>

    <div>
      <plan-card></plan-card>
    </div>

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

  .plan-container > div {
    width: 320px;
    margin: 0 16px;
  }

</style>
