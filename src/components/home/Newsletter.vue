<template>
  <div class="app-section newsletter">
    <div class="text-center mb-3">Subscribe to our newsletter</div>
    <div class="row">
      <div class="col-md-6 d-flex align-items-center justify-content-center mx-auto">
        <div>
          <input class="newsletter-form-input" type="text">
        </div>
        <div>
          <button class="newsletter-form-button">Subscribe</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style>
  .app-section.newsletter{
    background: url("../../../public/images/newsletter.png");
    color: var(--white);
  }
  .newsletter-form-input{
    height: 47px;
    width: 300px;
  }
  .newsletter-form-input:focus,
  .newsletter-form-input:active{
    outline: none;
  }
  .newsletter-form-button{
    text-decoration: none;
    color: var(--white);
    background: var(--black);
    padding: 15px 50px;
    font-size: 13px;
    font-weight: bolder;
    border-radius: 3px;
    border: none;
  }
  @media screen and (max-width: 600px) {
    .newsletter-form-input{
      width: 200px;
    }
    .newsletter-form-button{
      padding: 15px 20px;
    }
  }
  @media screen and (max-width: 400px) {
    .newsletter-form-input{
      width: 180px;
    }
    .newsletter-form-button{
      padding: 15px 20px;
    }
  }
</style>