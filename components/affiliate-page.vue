<template>
  <div class="container">
    <div class="affiliate-container">
      <div class="affiliate-title" style="text-align: initial">
        Join Our
        <div style="text-transform: uppercase">Affiliate Program</div>
        <img src="~/assets/images/horn-affiliate-marketing.png" alt="">
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "affiliate-page"
  }
</script>

<style scoped>
  .container {
    background-color: #2B2D42;
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    /*flex-direction: row-reverse;*/
    align-items: center;
    text-align: center;
    position: relative;
  }

  .container .affiliate-container {

    min-width: 58%;
    min-height: inherit;

    display: inherit;
    justify-content: center;
    align-items: center;
  }

  .affiliate-title {
    letter-spacing: 0;
    color: #FFFFFF;
    font-size: 56px;
    font-weight: 500;
  }

  .affiliate-title > div {
    line-height: 1;
  }

  .affiliate-title > img {
    max-width: 400px;
    /*height: 150px;*/
  }

</style>
