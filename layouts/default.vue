<template>
  <div>
    <top-header />
    <main id="main" role="main" class="container mx-auto">
      <nuxt />
    </main>
    <bottom-footer />
  </div>
</template>

<script>
import TopHeader from '~/components/TopHeader.vue';
import BottomFooter from '~/components/BottomFooter.vue';

export default {
  components: {
    TopHeader,
    BottomFooter
  }
}
</script>

<style lang="scss">
@import '../assets/scss/styles.scss';
</style>