<template>
  <div>
    <work
      :screen-shots="['/works/portfolio/figure0.png']"
      :technologies="['HTML/CSS', 'Vue.js', 'Nuxt.js', 'Element UI', 'CircleCI']"
      title="ポートフォリオサイト"
      date="2018/6"
      description="Nuxt.jsを利用したポートフォリオサイト．UIライブラリとしてElement UIを利用．これまでに作ったものや，撮影した写真を掲載．作成したページは，CircleCIを用いて自動ビルド/デプロイしている．"
      source-address="https://github.com/hama1080/portfolio"
    />
  </div>
</template>

<script>
import work from './work.vue'

export default {
  name: 'Portfolio',
  components: {
    work
  }
}
</script>

<style scoped>

</style>
