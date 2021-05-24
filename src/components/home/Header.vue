<template>
  <div class="row header">
    <div class="col-md-6 my-auto">
      <div>
        <div class="header-title">
          <span class="heavy">Together</span>, let's <span class="heavy">end</span> <br> the virus
        </div>
        <div class="header-info">Let’s all come together to support the health workers and destroy the pandemic</div>
        <a class="action-button" href="#">Test Now</a>
      </div>
    </div>
    <div class="col-md-6 d-md-block d-none text-right">
      <img class="header-image" :src="'/images/header.jpg'" alt="Header-Image">
    </div>
    <div class="col-12 scroll-down text-center">
      <img :src="'/images/scroll-down.svg'" alt="scroll-down">
    </div>
  </div>
</template>

<script>
  export default {

  }
</script>

<style>
  .header{
    padding: 100px 30px 100px 100px;
    background: var(--black);
    color: var(--white);
    font-weight: lighter;
  }
  .header-title{
    font-size: 50px;
    line-height: 58px;
    font-weight: lighter;
  }
  .header-info{
    margin: 30px 0;
    font-size: 16px;
  }
  .header-title .heavy{
    font-weight: 700;
  }
  .header .header-image{
    height: 500px;
  }
  .action-button{
    text-decoration: none;
    color: var(--white);
    background: var(--purple);
    padding: 15px 50px;
    font-size: 13px;
    font-weight: bolder;
    border-radius: 3px;
  }
  .action-button:hover{
    text-decoration: none;
    color: var(--white);
    background: var(--purple-hover);
  }
  @media screen and (max-width: 767px) {
    .header{
      padding: 300px 100px;
      background: url("../../../public/images/header.jpg") center/cover no-repeat, #000000;
    }
    .scroll-down{
      margin-top: 100px !important;
    }
  }
  @media screen and (max-width: 650px) {
    .header{
      padding: 300px 50px;
    }
  }
  @media screen and (max-width: 500px) {
    .header{
      padding: 300px 30px;
    }
  }
</style>