<template>
    <nav>
      <a href="/">Home</a>
      <a href="#about">About</a>
      <a href="#affiliate">Affiliate</a>
      <a href="#service">Service</a>
      <a href="#contact">Contact</a>
      <a href="#blog">Blog</a>
      <a href="#login">Login</a>
      <a href="#team">Team</a>
    </nav>
</template>

<script>
    export default {
        name: "header-home"
    }
</script>

<style scoped>
  nav{
    position: fixed;
    top: 0;
    z-index: 200;
    left: 0;

    width: 100%;
    height: 100px;
    background: #2B2D42 0 0 no-repeat padding-box;
    box-shadow: 10px 10px 6px #00000029;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  nav > a{
    font-size: 24px;
    letter-spacing: 5px;
    color: #FFFFFF;

    padding: 0 16px;
  }
</style>
