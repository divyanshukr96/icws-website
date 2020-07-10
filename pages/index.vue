<template>
  <div>
    <header-home v-bind:navOpen="navOpen" v-bind:toggleNav="toggleNav"></header-home>
    <home-page v-bind:toggleNav="toggleNav"></home-page>
    <about-page></about-page>
    <plan-page></plan-page>
    <service-page></service-page>
    <affiliate-page></affiliate-page>
    <contact-us-page></contact-us-page>
  </div>
</template>

<script>
  import HomePage from "../components/home-page";
  import AboutPage from "../components/about-page";
  import ServicePage from "../components/service-page";
  import ContactUsPage from "../components/contact-us-page";
  import AffiliatePage from "../components/affiliate-page";
  import PlanPage from "../components/plan-page";
  import HeaderHome from "../components/header-home";

  export default {
    components: {HeaderHome, PlanPage, AffiliatePage, ContactUsPage, ServicePage, AboutPage, HomePage},

    data: function () {
      return {
        navOpen: false,
      }
    },
    methods: {
      toggleNav() {
        this.navOpen = !this.navOpen;
      }
    }

  }
</script>

<style scoped>
  /*.container {*/
  /*  background-color: #2B2D42;*/
  /*  margin: 0 auto;*/
  /*  min-height: 100vh;*/
  /*  display: flex;*/
  /*  !*flex-direction: row-reverse;*!*/
  /*  align-items: center;*/
  /*  text-align: center;*/
  /*  position: relative;*/
  /*}*/

  /*.container > .home-container {*/
  /*  background-color: #FAA916;*/
  /*  width: 42%;*/
  /*  float: right;*/
  /*  min-height: inherit;*/

  /*  display: inherit;*/
  /*  justify-content: center;*/
  /*  align-items: center;*/

  /*}*/

  /*.title {*/
  /*  text-align: initial;*/
  /*  font-size: 56px;*/
  /*  white-space: pre-line;*/
  /*  line-height: 1;*/
  /*  color: #eee;*/
  /*  font-weight: 500;*/
  /*  margin-bottom: 16px;*/
  /*}*/

  /*.title span {*/
  /*  font-size: 72px;*/
  /*  text-transform: uppercase;*/
  /*}*/

  /*.home {*/
  /*  display: flex;*/
  /*  justify-content: center;*/
  /*}*/


  /*.btn {*/
  /*  margin-top: 30px;*/

  /*  height: 75px;*/
  /*  width: 280px;*/
  /*  font-size: 28px;*/

  /*  background: #2B2D42 0% 0% no-repeat padding-box;*/
  /*  color: #eee;*/
  /*}*/

  /*.quotes {*/
  /*  white-space: pre-line;*/
  /*  text-align: initial;*/

  /*  margin-top: 64px;*/
  /*  padding: 16px;*/

  /*  font-size: 48px;*/
  /*  line-height: 1.1;*/
  /*  text-transform: uppercase;*/
  /*  color: #eee;*/
  /*  font-weight: 400;*/
  /*}*/

  /*.quotes span {*/
  /*  text-transform: initial;*/
  /*}*/

  /*.home-navbar {*/
  /*  position: absolute;*/
  /*  top: 32px;*/
  /*  left: 60px;*/
  /*  right: 60px;*/
  /*  height: 80px;*/

  /*  display: flex;*/
  /*  align-items: center;*/


  /*}*/

  /*.home-navbar > div {*/
  /*  display: flex;*/
  /*  width: 100%;*/
  /*  align-items: center;*/

  /*}*/

  /*.home-navbar a {*/
  /*  font-size: 20px;*/
  /*  padding: 0 18px;*/
  /*  color: #eee;*/
  /*}*/


  /*.menu-icon {*/
  /*  width: 44px;*/
  /*  height: 44px;*/
  /*  background: #2B2D42 0% 0% no-repeat padding-box;*/
  /*  opacity: 1;*/
  /*  padding-top: 12px;*/
  /*  transform: rotate(-90deg);*/


  /*  margin: 0 16px;*/
  /*}*/

  /*.menu-icon span {*/
  /*  background: #2B2D42 0% 0% no-repeat padding-box;*/
  /*  border: 1px solid #FFFFFF;*/
  /*  opacity: 1;*/
  /*  margin: 2px;*/
  /*}*/

</style>


