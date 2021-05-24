<template>
  <div>
    <app-home-header/>
  </div>
</template>

<script>
// @ is an alias to /src
import appHomeHeader from '@/components/home/Header';

export default {
  name: 'Home',
  components: {
    appHomeHeader
  }
}
</script>
