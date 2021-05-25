<template>
  <div>
    <app-home-header/>
    <app-home-blog/>
    <app-home-testimonies/>
    <app-home-gallery/>
    <app-home-newsletter/>
  </div>
</template>

<script>
import appHomeHeader from '@/components/home/Header';
import appHomeBlog from '@/components/home/Blog';
import appHomeTestimonies from '@/components/home/Testimonies';
import appHomeGallery from '@/components/home/Gallery';
import appHomeNewsletter from '@/components/home/Newsletter';

export default {
  name: 'Home',
  components: {
    appHomeHeader,
    appHomeBlog,
    appHomeTestimonies,
    appHomeGallery,
    appHomeNewsletter
  }
}
</script>
