<template>
  <div id="app">
    <div id="navbar">
      <nav>
        <a href="#" class="brand-name">COVI<span>SOFT</span></a>
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
        </div>
      </nav>
    </div>
    <router-view/>
  </div>
</template>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Padauk:wght@400;700&display=swap');
  #app{
    font-family: 'Padauk', sans-serif;
  }
  #navbar{
    position: absolute;
    top: 0;
    width: 100%;
    background: #000;
  }
  nav{
    display: flex;
    justify-content: space-between;
    margin: 56px 100px;
  }
  nav .brand-name{
    color: #7D00A9;
    font-weight: 700;
    font-size: 18px;
    line-height: 22px;
    letter-spacing: 1px;
    text-decoration: none;
  }
  nav .brand-name span{
    color: #ffffff;
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
    color: #ffffff;
  }
</style>
