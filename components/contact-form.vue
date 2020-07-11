<template>
  <div class="contact-form">
    <div class="input-group">
      <input id="name" type="text" required/>
      <label for="name">Name</label>
    </div>
    <div class="input-group">
      <input id="email" type="text" required/>
      <label for="email">Email</label>
    </div>
    <div class="textarea">
      <label for="message">Message</label>
      <textarea id="message"></textarea>
    </div>
    <button>Send</button>
  </div>
</template>

<script>
  export default {
    name: "contact-form",
    computed: {
      isActive: function (eve) {
        console.log('---------------')
        console.log(eve)
      }
    },
    methods: {
      focusFun({target}) {
        console.log(target.value)
      }
    }
  }
</script>

<style scoped>

  .contact-form {
    text-align: initial;
    padding: 8px;
  }

  .input-group {
    position: relative;
    margin-bottom: 20px;
  }

  input {
    font-size: 18px;
    color: #2B2D42;
    font-weight: 500;
    padding: 8px 8px 8px 5px;
    display: block;
    width: 100%;
    border: none;
    border-bottom: 1px solid #707070;
  }

  input:focus {
    outline: none;
  }

  label {
    color: #715F5F;
    font-size: 18px;
    font-weight: normal;
  }

  .input-group > label {
    position: absolute;
    pointer-events: none;
    left: 5px;
    top: 10px;
    transition: 0.2s ease all;
    -moz-transition: 0.2s ease all;
    -webkit-transition: 0.2s ease all;
  }

  input:focus ~ label, input:valid ~ label {
    top: -16px;
    font-size: 14px;
    color: #715F5F;
  }

  textarea {
    width: 100%;
    margin-top: 8px;
    height: 200px;
    border-radius: 12px;
    background: #F0E6E6 0 0 no-repeat padding-box;
    padding: 10px;
    border: none;

    font-size: 16px;
    color: #2B2D42;
  }

  textarea:focus {
    border: 1px solid #70707070;
    outline: none;
  }

  .textarea {
    margin-bottom: 18px;
  }

  .textarea > label {
    padding-left: 6px;
    font-size: 18px;
  }

  .contact-form button {
    margin-left: 50%;
    transform: translateX(-50%);
    text-transform: uppercase;
    font-size: 18px;
    font-weight: 500;
    color: #fff;
    height: 40px;
    width: 140px;
    background: #FAA916 0 0 no-repeat padding-box;
    border-radius: 15px;
    border: none;
    transition: all .25s ease;
    cursor: pointer;
  }

  .contact-form button:focus {
    outline: none;
  }
  .contact-form button:hover {
    -webkit-box-shadow: 1px 2px 4px 0 rgba(0,0,0,0.75);
    -moz-box-shadow: 1px 2px 4px 0 rgba(0,0,0,0.75);
    box-shadow: 1px 2px 4px 0 rgba(0,0,0,0.75);
  }

</style>


