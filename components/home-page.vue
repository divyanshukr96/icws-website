<template>
  <div class="container">
    <div class="home-navbar">
      <a href="" class="icws-logo"><img src="~/assets/images/icws-logo.png" alt=""></a>
      <div style="flex-grow: 1"></div>
      <div class="navigation-menu">
        <a href="/">Home</a>
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#contact">contact</a>
      </div>
      <div class="menu-icon" @click.prevent="toggleNav">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>
    <div style="position: absolute; bottom:8px; left: 50%; transform: translateX(-50%)">
      <img src="~/assets/images/mouse.svg" alt="mouse">
    </div>
    <div class="home-container">
      <div class="home">
        <div class="title">Your
          <span>Website</span>
        </div>
        <div class="quotes">
          <span>on</span>
          Easy
          Monthly
          installments
        </div>
        <button class="btn button--green">View Details</button>
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
    height: 100vh;
    min-height: 500px;
    display: flex;
    flex-direction: row-reverse;
    align-items: center;
    text-align: center;
    position: relative;
  }

  .home-container {
    background-color: #FAA916;
    width: 58%;
    float: right;
    height: inherit;
    min-height: inherit;

    display: inherit;
    justify-content: center;
    align-items: center;

  }

  .navigation-menu {
    transition: all .5s ease;
  }

  .icws-logo {
    padding: 8px;
  }

  .icws-logo > img {
    height: 56px;
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
  }

  .title span {
    font-size: 72px;
    text-transform: uppercase;
  }

  .home {
    position: relative;
    display: flex;
    justify-content: center;
  }


  .home > .btn {
    margin-top: 20px;
    height: 120px;
    width: 270px;
    max-width: 100%;
    font-size: 28px;

    background: #2B2D42 0 0 no-repeat padding-box;
    color: #eee;

    position: absolute;
    left: 12px;
    bottom: 0;
  }

  .quotes {
    white-space: pre-line;
    text-align: initial;

    margin-top: 64px;
    padding: 0 16px;

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


    transition: all .5s ease;

  }


  .home-navbar div a {
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

  @media only screen and (max-width: 1200px) {

    .home > .btn {
      left: 0;
      width: 220px;
      max-height: 110px;
    }

    .title {
      font-size: 40px;
    }

    .title span {
      font-size: 54px;
    }

    .quotes {
      font-size: 36px;
    }
  }

  @media only screen and (max-width: 900px) {
    .home-navbar {
      top: 0;
      left: 0;
      width: 100%;
    }

    .home > .btn {
      transform: translateY(calc(100% + 16px));
      max-height: 48px;
      padding: unset;
      font-size: 22px;
    }

    .home {
      flex-direction: column;
      z-index: 2;
    }

    .title {
      font-size: 36px;
    }

    .title span {
      font-size: 48px;
    }

    .quotes {
      font-size: 28px;
      margin-left: -16px;
      margin-top: 8px;
    }
  }


  @media only screen and (max-width: 600px) {

    .home-navbar .navigation-menu {
      display: none;
    }

    .home-container {
      width: 100%;
    }

    .home {
      flex-direction: column;
      z-index: 2;
    }


    .home-image {
      position: absolute;
      top: 0;
      left: 0;
      height: 100vh;
      width: 100%;
      display: flex;
      z-index: 0;
    }

    .home-image > img {
      opacity: .6;
    }

    .title {
      font-size: 36px;
    }

    .title span {
      font-size: 48px;
    }

    .quotes {
      font-size: 28px;
      margin-left: -16px;
      margin-top: 8px;
    }
  }

</style>
