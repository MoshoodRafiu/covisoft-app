<template>
  <div>
    <app-home-header/>
    <app-home-blog/>
    <app-home-testimonies/>
  </div>
</template>

<script>
// @ is an alias to /src
import appHomeHeader from '@/components/home/Header';
import appHomeBlog from '@/components/home/Blog';
import appHomeTestimonies from '@/components/home/Testimonies';

export default {
  name: 'Home',
  components: {
    appHomeHeader,
    appHomeBlog,
    appHomeTestimonies
  }
}
</script>
