<template>
  <div>
    <work
      :screen-shots="['/works/analogSynthesizer/figure0.jpg', '/works/analogSynthesizer/figure1.jpg', '/works/analogSynthesizer/figure2.jpg']"
      :technologies="['Electronics']"
      title="Analog Synthesizer"
      date="2018/12"
      description="
      <a href='https://www.oreilly.co.jp/books/9784873117515/'>Make: Analog Synthesizers</a>を参考に作ったアナログシンセサイザー。
      つまみを回すことで、様々な音を奏でることが出来る。
      部品は<a href='http://akizukidenshi.com/catalog/g/gK-12334/'>秋月電子のキット</a>を利用。
      ケースはダンボールを切り抜いて作成。
      "
    />
  </div>
</template>

<script>
import work from './work.vue'

export default {
  name: 'AnalogSynthesizer',
  components: {
    work
  }
}
</script>

<style scoped>
</style>
