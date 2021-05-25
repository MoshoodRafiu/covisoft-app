<template>
  <div class="app-section light row">
      <div class="col-12 app-section-title-wrapper">
        <div class="app-section-title dark">Recent Blog Posts</div>
      </div>
      <div class="col-12">
        <div class="row">
          <app-blog-post v-for="post in posts" :key="post.title"
            :author="post.author"
            :title="post.title"
            :image-src="post.src"
          />
        </div>
      </div>
      <div class="col-12 more-post-button text-center">
        <a class="action-button" href="#">More Posts</a>
      </div>
  </div>
</template>

<script>
  import appBlogPost from "../BlogPost";
  export default {
    data(){
      return{
        posts: [
          { author: 'By Shalom Asenuga', title: 'The Covid Situation in India', src: '/images/blog/1.png' },
          { author: 'By Michael Townley', title: 'Local people support the COVID Initiative', src: '/images/blog/2.png' },
          { author: 'By Leslie Williams', title: 'Doctors In Distress!!', src: '/images/blog/3.png' },
          { author: 'By Shalom Asenuga', title: 'Businesses are out!', src: '/images/blog/4.png' },
          { author: 'By Michael Townley', title: 'Russia reportedly discovers cure', src: '/images/blog/5.png' },
        ]
      }
    },
    components: {
      appBlogPost
    }
  }
</script>

<style>
  .app-section{
    padding: 60px 100px;
  }
  .app-section.light{
    background: var(--white);
  }
  .app-section.dark{
    background: var(--black);
  }
  .app-section-title{
    font-size: 38px;
    font-weight: 700;
    padding-left: 10px;
    line-height: 45px;
    margin-bottom: 60px;
  }
  .app-section-title.dark{
    color: var(--black);
    border-left: 6px solid var(--black);
  }
  .app-section-title.light{
    color: var(--white);
    border-left: 6px solid var(--white);
  }
  @media screen and (max-width: 650px) {
    .app-section{
      padding: 60px 50px;
    }
  }
  @media screen and (max-width: 500px) {
    .app-section-title-wrapper{
      padding: 0 !important;
    }
    .app-section{
      padding: 60px 30px;
    }
    .more-post-button{
      margin-top: 50px !important;
    }
  }
</style>