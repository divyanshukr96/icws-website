<template>
  <div class="container">

    <div>
      <service-card></service-card>
    </div>
    <div>
      <service-card></service-card>
    </div>
    <div>
      <service-card></service-card>
    </div>
    <div>
      <service-card></service-card>
    </div>
    <div>
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
  .container {
    background-color: #FAA916 !important;
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    /*flex-direction: row-reverse;*/
    align-items: initial !important;
    text-align: center;
    position: relative;

    justify-content: center;



    padding: 64px 48px;
  }

  .container > div {
    width: 220px;
    margin: 0 8px;
  }

  .container > div:nth-child(even) {
    align-self: flex-end;
  }


</style>
