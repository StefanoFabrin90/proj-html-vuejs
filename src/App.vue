<template>
  <div id="app">
    <!-- HEADER -->
    <header>
      <!-- section-1 header -->
      <Sec1Header />

    </header>
  </div>
</template>

<script>
import Sec1Header from '@/components/Sec1Header.vue';

export default {
  name: 'App',
  components: {
    Sec1Header,
  }
}
</script>

<style lang="scss">
* {
  font-family: sans-serif;
}
</style>
