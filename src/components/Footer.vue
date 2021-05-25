<template>
  <div class="app-section footer dark row">
    <div class="col-md-7">
      <a href="#" class="brand-name">
        <img :src="'/images/logo.svg'" class="brand-logo" alt="logo">
        COVI<span>SOFT</span>
      </a>
      <div class="brand-info">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quaerat quasi quo velit voluptatem! Ab adipisci, corporis, debitis doloremque, doloribus excepturi harum iure iusto libero minus nulla quisquam sequi voluptate. Nemo.
      </div>
    </div>
    <div class="col-md-5">
      <ul class="quicklinks">
        <li>
          <a href="#">Career</a>
        </li>
        <li>
          <a href="#">Donate</a>
        </li>
        <li>
          <a href="#">About Us</a>
        </li>
        <li>
          <a href="#">Contact Us</a>
        </li>
      </ul>
    </div>
    <div class="col-12 copyright-text">
      &copy; All right reserved {{ year }} COVISOFT
    </div>
  </div>
</template>

<script>
  export default {
    data(){
      return{
        year: (new Date).getFullYear()
      }
    }
  }
</script>

<style>
  .footer div .brand-name{
    color: var(--purple);
    font-weight: 700;
    font-size: 24px;
    line-height: 22px;
    letter-spacing: 1px;
    text-decoration: none;
  }
  .footer div .brand-name:hover{
    color: var(--purple);
  }
  .footer div .brand-name span{
    color: var(--white);
  }
  .footer div .brand-name .brand-logo{
    width: 40px;
  }
  .brand-info{
    margin: 10px 0;
    color: var(--white);
    font-weight: lighter;
    font-size: 14px;
  }
  ul.quicklinks {
    padding: 0;
    margin: 0;
  }
  ul.quicklinks li{
    list-style: none;
    text-align: right;
    margin-top: 10px !important;
  }
  ul.quicklinks li a{
    text-decoration: none;
    color: var(--white);
    font-size: 14px;
  }
  ul.quicklinks li a:hover{
    text-decoration: none;
    color: var(--purple);
  }
  .copyright-text{
    margin-top: 25px !important;
    color: #B8B8B8;
    font-size: 13px;
  }
  @media screen and (max-width: 767px) {
    ul.quicklinks li{
      margin-top: 20px;
      text-align: left;
    }
  }
</style>