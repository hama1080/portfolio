<template>
  <div>
    <work
      :screen-shots="['/works/portfolio/figure0.png']"
      :technologies="['HTML/CSS', 'Vue.js', 'Nuxt.js', 'Element UI', 'CircleCI']"
      title="ポートフォリオサイト"
      date="2018/6"
      description="
      Vue.js/Nuxt.jsの練習用に作成したポートフォリオサイト。
      UIライブラリとしてElement UIを利用。
      これまでに作ったものや、撮影した写真を掲載。
      作成したページは、CircleCIを用いて自動ビルド/デプロイしている。
      ページが増えるにつれて気になる箇所が多くなってきたため、改修する予定。
      "
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
