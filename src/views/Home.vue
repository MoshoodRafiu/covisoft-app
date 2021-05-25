<template>
  <div>
    <app-home-header/>
    <app-home-blog/>
    <app-home-testimonies/>
    <app-home-gallery/>
  </div>
</template>

<script>
import appHomeHeader from '@/components/home/Header';
import appHomeBlog from '@/components/home/Blog';
import appHomeTestimonies from '@/components/home/Testimonies';
import appHomeGallery from '@/components/home/Gallery';

export default {
  name: 'Home',
  components: {
    appHomeHeader,
    appHomeBlog,
    appHomeTestimonies,
    appHomeGallery
  }
}
</script>
