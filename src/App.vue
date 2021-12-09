<template>
  <div id="app">
    <!-- HEADER -->
    <header>
      <!-- section-1 header -->
      <Sec1Header />
      <!-- section-2 header -->
      <Sec2Header />
      <!-- Hero -->
      <Hero />
    </header>
  </div>
</template>

<script>
import Sec1Header from '@/components/Sec1Header.vue';
import Sec2Header from '@/components/Sec2Header.vue';
import Hero from '@/components/Hero.vue';

export default {
  name: 'App',
  components: {
    Sec1Header,
    Sec2Header,
    Hero,
  }
}
</script>

<style lang="scss">
* {
  font-family: sans-serif;
}
</style>
