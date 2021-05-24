<template>
  <div>
    <app-home-header/>
    <app-home-blog/>
  </div>
</template>

<script>
// @ is an alias to /src
import appHomeHeader from '@/components/home/Header';
import appHomeBlog from '@/components/home/Blog';

export default {
  name: 'Home',
  components: {
    appHomeHeader,
    appHomeBlog
  }
}
</script>
