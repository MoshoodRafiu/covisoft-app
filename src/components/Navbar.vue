<template>
  <div id="navbar">
    <nav>
      <a href="#" class="brand-name">
        <img :src="'/images/logo.svg'" class="brand-logo" alt="logo">
        COVI<span>SOFT</span>
      </a>
      <div>
        <ul>
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
        <div class="toggle">
          <div class="line-1"></div>
          <div class="line-2"></div>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>

</script>

<style>
  #navbar{
    position: absolute;
    top: 0;
    width: 100%;
    background: var(--black);
  }
  nav{
    display: flex;
    justify-content: space-between;
    margin: 40px 100px;
  }
  nav .brand-name{
    color: var(--purple);
    font-weight: 700;
    font-size: 28px;
    line-height: 22px;
    letter-spacing: 1px;
    text-decoration: none;
  }
  nav .brand-name .brand-logo{
    width: 40px;
  }
  nav .brand-name:hover{
    color: var(--purple);
  }
  nav .brand-name span{
    color: var(--white);
  }
  nav ul{
    padding: 0;
    margin: 0;
  }
  nav ul li{
    list-style: none;
    display: inline-block;
    margin: 0 40px;
  }
  nav ul li a{
    text-decoration: none;
    color: var(--white);
    font-size: 14px;
  }
  nav ul li a:hover{
    text-decoration: none;
    color: var(--purple);
  }
  .toggle{
    padding: 5px;
    display: none;
  }
  .toggle .line-1,
  .toggle .line-2{
    height: 4px;
    background: var(--white);
    border-radius: 5px;
    margin: 5px;
  }
  .toggle .line-1{
    width: 30px;
    margin-left: auto;
  }
  .toggle .line-2{
    width: 20px;
    margin-left: auto;
  }
  @media screen and (max-width: 1000px) {
    nav ul{
      display: none;
    }
    .toggle{
      display: block;
    }
  }
  @media screen and (max-width: 650px) {
    nav{
      margin: 40px 50px;
    }
  }
  @media screen and (max-width: 500px) {
    nav{
      margin: 40px 30px;
    }
  }
</style>