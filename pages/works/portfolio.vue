<template>
  <div>
    <work
      title="ポートフォリオサイト"
      date="2018/6"
      description="Nuxt.jsを利用したポートフォリオサイト．UIライブラリとしてElement UIを利用．これまでに作ったものや，撮影した写真を掲載．"
      v-bind:screenShots="['/works/portfolio/figure0.png']"
      v-bind:technologies="['HTML/CSS', 'Vue.js', 'Nuxt.js', 'Element UI']"
      sourceAddress="https://github.com/hama1080/portfolio"
    ></work>
  </div>
</template>

<script>
import work from './work.vue'

export default {
  name: 'portfolio',
  components: {
    work
  }
}
</script>

<style scoped>

</style>
