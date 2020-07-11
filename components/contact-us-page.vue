<template>
  <div class="container">
    <div class="contact-container">
      <div class="contact-form-container">
        <div><span>Send us any query</span></div>
        <div class="contact-form">
          <contact-form></contact-form>
        </div>
      </div>
    </div>
    <div class="contact-title">
      <div style="width: max-content">
        <div class="title">Contact Us</div>
        <div>icon<span>pthapli999@gmail.com</span></div>
        <div>icon<span>+91 8699665117</span></div>
      </div>
    </div>
  </div>
</template>

<script>
  import ContactForm from "./contact-form";
  export default {
    name: "contact-us-page",
    components: {ContactForm}
  }
</script>

<style scoped>
  .container {
    background-color: #FAA916 !important;
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    flex-direction: row-reverse;
    align-items: center;
    text-align: center;
    position: relative;
  }


  .container > .contact-container {
    background-color: #2B2D42;
    min-width: 58%;
    min-height: inherit;

    display: inherit;
    justify-content: center;
    align-items: center;

  }

  .contact-title {
    padding: 64px;
    width: 100%;
    text-align: initial;

    display: flex;
    justify-content: center;
    color: #eee;
  }


  .contact-title .title {
    text-align: initial;
    font-size: 72px;
    white-space: pre-line;
    line-height: 1;
    color: #eee;
    font-weight: 500;
    margin-bottom: 16px;
  }

  .contact-title div > span {
    letter-spacing: 0;
    color: #FFFFFF;
    font-size: 28px;
  }

  .contact-form-container {
    background: #FAA916 0 0 no-repeat padding-box;
    border: 1px solid #707070;
    border-radius: 20px;
    width: 360px;
  }

  .contact-form-container > div:first-child {
    padding: 12px 0;
  }

  .contact-form-container > div span {
    font-size: 28px;
    letter-spacing: 0;
    color: #FFFFFF;
  }

  .contact-form-container > .contact-form {
    background: #FFFFFF 0 0 no-repeat padding-box;
    /*border: 1px solid #707070;*/
    border-radius: 20px;
    padding: 20px;
  }

</style>
