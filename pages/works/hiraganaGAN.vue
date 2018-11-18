<template>
  <div>
    <work
      :screen-shots="['/works/hiraganaGAN/learning_flow.gif', '/works/hiraganaGAN/learning_result.png']"
      :technologies="['Python', 'Keras(TensorFlow)', 'Conditional GAN']"
      title="ひらがなGAN"
      date="2018/3"
      description="
      <a href='http://dl4us.com/'>DL4US</a>の課題で実施した、GANを用いた手書きひらがな文字の生成。
      学習には、産業技術総合研究所が公開している、ETL文字データベースを利用した。
      学習後に任意のひらがな文字を生成可能とするため、ネットワーク構造にはConditional GANを利用している。"
      source-address=""
    />
  </div>
</template>

<script>
import work from './work.vue'

export default {
  name: 'HiraganaGAN',
  components: {
    work
  }
}
</script>

<style scoped>

</style>
