<script setup>
</script>

<template>
  <div class="tw-layout">
    <TheLayout></TheLayout>
  </div>
</template>

<script>
import TheLayout from './layout/TheLayout.vue';
export default {
  components: {
    TheLayout
  }
}
</script>


<style lang="scss">

* {
    margin: 0;
    padding: 0;
    // font-family: 'IBM Plex Sans Thai' !important;
    color: #333;
}

.tw-layout {
  height: 100vh;
  overflow: hidden;
}

html,
body {
  height: 100%;
  .layout-boxed & {
    height: 100%;
  }
}

body {
  font-weight: 400;
  overflow-x: hidden;
  overflow-y: auto;
  line-height: inherit;
}

</style>
