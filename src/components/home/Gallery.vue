<template>
  <div class="app-section light row">
    <div class="col-12 app-section-title-wrapper">
      <div class="app-section-title dark">Gallery</div>
    </div>
    <div class="col-12">
      <div class="row">
        <div v-for="(image, index) in currentImages" :key="image+index" class="col-md-3 col-6">
          <img :src="image" class="gallery-image" alt="gallery-image">
        </div>
      </div>
    </div>
    <img v-if="start !== 0" class="gallery-prev" @click="getPreviousImage" :src="'images/gallery-prev.svg'" alt="gallery-prev">
    <img v-if="end < images.length" class="gallery-next" @click="getNextImage" :src="'images/gallery-next.svg'" alt="gallery-next">
  </div>
</template>

<script>
  export default {
    data(){
      return{
        start: 0,
        end: 4,
        images: [
            'images/gallery/1.png', 'images/gallery/2.png', 'images/gallery/3.png', 'images/gallery/4.png',
            'images/gallery/1.png', 'images/gallery/2.png', 'images/gallery/3.png', 'images/gallery/4.png',
        ],
        currentImages: []
      }
    },
    mounted() {
      if (window.innerWidth < 768){
        this.end = 2
      }
      this.getCurrentImages();
    },
    methods: {
      getNextImage(){
        if (this.images.length > this.end){
          this.start++;
          this.end++;
          this.getCurrentImages();
        }
      },
      getPreviousImage(){
        console.log('Prev')
        if (this.start > 0){
          this.start--;
          this.end--;
          this.getCurrentImages();
        }
      },
      getCurrentImages(){
        this.currentImages = this.images.slice(this.start, this.end);
      }
    }
  }
</script>

<style>
  .gallery-image{
    width: 100%;
    margin-bottom: 50px;
  }
  .gallery-prev, .gallery-next{
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    width: 70px !important;
    cursor: pointer;
  }
  .gallery-next{
    right: 10px;
  }
  .gallery-prev{
    left: 10px;
  }
</style>