<template>
  <nav v-bind:style="{display: display ? 'none' : 'flex'}">
    <a href="/">Home</a>
    <a href="#about">About</a>
    <a href="#affiliate">Affiliate</a>
    <a href="#service">Service</a>
    <a href="#contact">Contact</a>
    <a href="#blog">Blog</a>
    <a href="#login">Login</a>
    <a href="#team">Team</a>
    <span v-if="display" class="close-navbar" @click="toggleNav"></span>
  </nav>
</template>

<script>
  export default {
    name: "header-home",
    props: {
      navOpen: Boolean,
      toggleNav: Function,
    },
    data() {
      return {
        display: true,
        navDisplay: 'none',
      }
    },
    computed: {
      isNavOpen: function () {
        return this.display;
      }
    },
    watch: {
      navOpen: function (value) {
        this.display = value;
      },
    },
    methods: {
      handleScroll(event) {
        this.display = (window.scrollY < 50);
        if (this.display) {
          this.navDisplay = 'none'
        } else {
          this.navDisplay = 'flex'
        }
      }
    },
    beforeMount() {
      window.addEventListener('scroll', this.handleScroll);
    },
    beforeDestroy() {
      window.removeEventListener('scroll', this.handleScroll);
    },
  }
</script>

<style scoped>
  nav {
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
    transition: all .5s ease;
  }

  .d-none {
    display: none;
  }

  nav > a {
    font-size: 20px;
    letter-spacing: 5px;
    color: #FFFFFF;

    padding: 0 16px;
  }

  nav .close-navbar {
    position: absolute;
    right: 70px;
    top: 50%;
    width: 28px;
    height: 28px;
    opacity: 0.7;
    transform: translateY(-50%);
    cursor: pointer;
  }

  nav .close-navbar:before, nav .close-navbar:after {
    position: absolute;
    left: 0;
    content: ' ';
    height: 28px;
    width: 2px;
    background-color: #eeeeee;
  }

  nav .close-navbar:before {
    transform: rotate(45deg);
  }

  nav .close-navbar:after {
    transform: rotate(-45deg);
  }

</style>
