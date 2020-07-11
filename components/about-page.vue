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
        <div class="details">
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
    width: 100%;
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
    font-size: 70px;
    line-height: 1;
    color: #eee;
    font-weight: 500;
  }

  .home-about .title {
    text-transform: uppercase;
    font-weight: bold;
  }

  .title.rotate {
    writing-mode: vertical-lr;
    transform: rotate(180deg);
    text-align: center;
  }

  .home {
    display: flex;
    justify-content: center;
  }


  .home-about {
    padding: 64px;
    width: inherit;
    /*text-align: initial;*/

    display: flex;
    flex-direction: row-reverse;
    justify-content: center;
    position: relative;
    color: #eee;
  }

  .home-about .content {
    max-width: 600px;
  }


  .content .details {
    padding: 8px 16px;
    font-size: 20px;
    text-align: justify;
  }

  @media only screen and (max-width: 1200px) {
    .home-about {
      padding: 32px;
    }

    .title {
      font-size: 58px;
      margin: 0;
    }

    .content .details {
      font-size: 18px;
    }
  }

  @media only screen and (max-width: 900px) {
    .container > .home-container {
      /*display: none;*/
    }

    .home-about {
      padding: 16px;
    }

    .title {
      font-size: 48px;
    }

    .content .details {
      padding: 8px;
      font-size: 17px;
    }

  }

  @media only screen and (max-width: 600px) {
    .container > .home-container {
      /*position: absolute;*/
      /*min-height: unset;*/
      /*top: 0;*/
      /*left: 0;*/
      /*width: 100%;*/
      /*height: 50%;*/
      display: none;
    }

    /*.container > .home-container > div {*/
    /*  display: none;*/
    /*}*/
    .title {
      font-size: 40px;
    }

    .content .details {
      font-size: 16px;
    }


  }

</style>
