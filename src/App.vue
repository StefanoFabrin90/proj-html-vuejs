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
      <!-- section-5 main -->
      <Sec5Main />
      <!-- section-6 main -->
      <Sec6Main />
      <!-- section-7 main -->
      <Sec7Main />
    </main>

    <!-- FOOTER -->
    <footer>
      <!-- section-1 footer -->
      <Sec1Footer />
    </footer>
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
import Sec5Main from '@/components/Sec5Main.vue';
import Sec6Main from '@/components/Sec6Main.vue';
import Sec7Main from '@/components/Sec7Main.vue';
import Sec1Footer from '@/components/Sec1Footer.vue';

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
    Sec5Main,
    Sec6Main,
    Sec7Main,
    Sec1Footer,
  }
}
</script>

<style lang="scss">
* {
  font-family: sans-serif;
  overflow-x: hidden;
}
</style>
