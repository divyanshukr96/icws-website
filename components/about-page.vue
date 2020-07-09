<template>
  <div class="container">
    <div class="home-container">
      <div class="home">
        <div class="title">About Us</div>
      </div>
    </div>
    <div class="home-about">
      <div class="content">
        <div class="title">Design</div>
        <div style=" padding: 8px 16px; font-size: 20px; text-align: justify;">
          Something about us will come here and will be formatted withing this box only so keep the word limit and rest
          of
          the content in mind. Rest all is gibberish from here on no need tro read this stuff. Avenir is one of my
          favourite font as it looks pretty cool. Helvetica is overrated. Lato does better than helvetica. Typography is
          an art and i am the artist. I think we should put some images on the website for visual pleasure. Maybe not.
        </div>
        <div class="title">Deliver</div>
      </div>
      <div class="title rotate">Develop</div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "about-page"
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

  .container > .home-container {
    background-color: #FAA916;
    min-width: 42%;
    min-height: inherit;

    display: inherit;
    justify-content: center;
    align-items: center;

  }

  .title {
    text-align: initial;
    font-size: 80px;
    white-space: pre-line;
    line-height: 1;
    color: #eee;
    font-weight: 500;
    margin-bottom: 16px;
  }

  .home-about .title {
    text-transform: uppercase;
    font-weight: bold;
  }

  .title.rotate {
    transform: rotate(-90deg) translateX(25%);
    min-height: 300px;
    bottom: 0;
    position: absolute;
  }

  .home {
    display: flex;
    justify-content: center;
  }


  .home-about {
    padding: 64px;
    width: fit-content;
    text-align: initial;

    display: flex;
    justify-content: end;
    position: relative;
    color: #eee;
  }

  .home-about .content {
    margin-left: 115px;
  }

</style>
