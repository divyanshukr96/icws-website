<template>
  <div class="container">
    <div class="home-navbar">
      <div>
        <a href="">ICWS</a>
        <div style="flex-grow: 1"></div>
        <a href="/">Home</a>
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#contact">contact</a>
        <div class="menu-icon" @click.prevent="toggleNav">
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>
    </div>
    <div style="position: absolute; bottom: 24px; left: 50%; transform: translateX(-50%)">
      <img src="~/assets/images/mouse.svg" alt="mouse">
    </div>
    <div class="home-container">
      <div class="home">
        <div>
          <div class="title">Your
            <span>Website</span></div>
          <button class="btn button--green">View Details</button>
        </div>
        <div class="quotes">
          <span>on</span>
          Easy
          Monthly
          installments
        </div>
      </div>
    </div>
    <div class="home-image">
      <img src="~/assets/images/new company vector 1.svg" alt="">
    </div>
  </div>
</template>

<script>
  export default {
    name: "home-page",
    props: {
      toggleNav: Function,
    },
  }
</script>

<style scoped>
  .container {
    background-color: #2B2D42;
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    flex-direction: row-reverse;
    align-items: center;
    text-align: center;
    position: relative;
  }

  .container > .home-container {
    background-color: #FAA916;
    width: 58%;
    float: right;
    min-height: inherit;

    display: inherit;
    justify-content: center;
    align-items: center;

  }

  .home-image {
    width: 42%;
  }

  .home-image img {
    width: 100%;
  }

  .title {
    text-align: initial;
    font-size: 56px;
    white-space: pre-line;
    line-height: 1;
    color: #eee;
    font-weight: 500;
    margin-bottom: 16px;
  }

  .title span {
    font-size: 72px;
    text-transform: uppercase;
  }

  .home {
    display: flex;
    justify-content: center;
  }


  .btn {
    margin-top: 20px;

    height: 120px;
    width: 280px;
    font-size: 28px;

    background: #2B2D42 0% 0% no-repeat padding-box;
    color: #eee;
  }

  .quotes {
    white-space: pre-line;
    text-align: initial;

    margin-top: 64px;
    padding: 16px;

    font-size: 48px;
    line-height: 1.1;
    text-transform: uppercase;
    color: #eee;
    font-weight: 500;
  }

  .quotes span {
    text-transform: initial;
  }

  .home-navbar {
    position: absolute;
    top: 10px;
    left: 60px;
    right: 60px;
    height: 80px;

    display: flex;
    align-items: center;


  }

  .home-navbar > div {
    display: flex;
    width: 100%;
    align-items: center;

  }

  .home-navbar a {
    font-size: 20px;
    padding: 0 18px;
    color: #eee;
  }


  .menu-icon {
    width: 44px;
    height: 44px;
    background: #2B2D42 0 0 no-repeat padding-box;
    padding-top: 12px;
    transform: rotate(-90deg);


    margin: 0 16px;
    cursor: pointer;
  }

  .menu-icon span {
    background: #2B2D42 0 0 no-repeat padding-box;
    border: 1px solid #FFFFFF;
    opacity: 1;
    margin: 2px;
  }


  @keyframes nav-slider {

  }

</style>
