<template>
  <div class="col-lg-4 blog-post col-sm-6">
    <a href="#" class="post-image">
      <img :src="imageSrc" class="img-fluid" alt="blog-post-image">
    </a>
    <div>
      <a href="#" class="post-title">
        {{ title}}
      </a>
    </div>
    <div class="post-author">
      {{ author}}
    </div>
  </div>
</template>

<script>
  export default {
    props: [
        'imageSrc', 'title', 'author'
    ]
  }
</script>

<style>
  .blog-post{
    margin-bottom: 100px;
  }
  .post-image img{
    margin-bottom: 10px;
  }
  .post-title{
    font-weight: 700;
    font-size: 17px;
    color: var(--black);
    text-decoration: none;
  }
  .post-title:hover{
    color: black;
  }
  .post-author{
    margin-top: 5px;
    font-weight: lighter;
    font-size: 13px;
  }
  @media screen and (max-width: 500px) {
    .blog-post{
      margin-bottom: 20px;
      border-bottom: 1px solid rgba(204, 204, 204, 0.9);
      padding: 0 0 30px 0 !important;
    }
    .blog-post:last-child{
      border: none !important;
    }
  }
</style>