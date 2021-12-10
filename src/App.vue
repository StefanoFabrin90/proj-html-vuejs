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


    <!-- MAIN -->
    <main>
      <!-- section-1 main -->
      <Sec1Main />
      <!-- section-2 main -->
      <Sec2Main />
      <!-- section-3 main -->
      <Sec3Main />
      <!-- section-4 main -->
      <Sec4Main />
    </main>
  </div>
</template>

<script>
import Sec1Header from '@/components/Sec1Header.vue';
import Sec2Header from '@/components/Sec2Header.vue';
import Hero from '@/components/Hero.vue';
import Sec1Main from '@/components/Sec1Main.vue';
import Sec2Main from '@/components/Sec2Main.vue';
import Sec3Main from '@/components/Sec3Main.vue';
import Sec4Main from '@/components/Sec4Main.vue';

export default {
  name: 'App',
  components: {
    Sec1Header,
    Sec2Header,
    Hero,
    Sec1Main,
    Sec2Main,
    Sec3Main,
    Sec4Main,
  }
}
</script>

<style lang="scss">
* {
  font-family: sans-serif;
  overflow-x: hidden;
}
</style>
