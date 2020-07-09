<template>
  <div class="card">
    <div class="card-title">Silver</div>
    <div>
      <p>For small portfolios and display websites</p>
      <p>Ticket based query</p>
      <p>Lorem Ipsum</p>
    </div>

    <h3>25$/month</h3>

    <div style="margin: 16px 0 4px;"><a href="#" class="btn">Get Started</a></div>
  </div>
</template>

<script>
  export default {
    name: "plan-card"
  }
</script>

<style scoped>
  .card {
    padding: 32px 40px;
    border-radius: 8px;

    background: #2B2D42 0 0 no-repeat padding-box;
    border: 1px solid #707070;
    color: #fff;
  }

  .card .card-title {
    font-size: 28px;
    letter-spacing: 6px;
    color: #FFFFFF;
    padding-bottom: 12px;
    text-transform: uppercase;
  }

  .card p {
    border-top: 1px solid #FFFFFF;
    padding-top: 12px;

    font-size: 18px;
  }

  .card p:last-child {
    border-bottom: 1px solid #FFFFFF;
    padding-bottom: 12px;
  }

  .card h3 {
    color: #fff;
    font-size: 20px;
    letter-spacing: 3px;
    padding-bottom: 12px;
  }


  .card .btn {
    background: #FFFFFF 0 0 no-repeat padding-box;
    border: 1px solid #707070;
    border-radius: 8px;
    padding: 8px 16px;

    text-decoration: none;
    letter-spacing: 2px;
    color: #2B2D42;
    font-size: 20px;
    font-weight: 500;
  }
</style>
