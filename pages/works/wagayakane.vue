<template>
  <div>
    <work
      :screen-shots="['/works/wagayakane/figure0.png']"
      :technologies="['Python', 'Raspberry Pi', 'MMD(Miku Miku Dance)']"
      title="我が家のあかねちゃんプロジェクト"
      date="2017/8"
      description="
      友人と共に実施した、我が家のあかねちゃんプロジェクト。
      自作スマートスピーカーのようなもので、Google HomeやAmazon Echoが大々的に発売される前に製作した。
      売り文句は、'ラズパイことraspberry piを使って音声認識やらTwitterから家電を操作できるやつを作ってみました'。
      詳細は<a href='http://wagayakane.html.xdomain.jp/index.html'>Webページ</a>や<a href='https://www.nicovideo.jp/watch/sm31762094'>動画</a>を参照。"
      source-address="https://github.com/hama1080/WagayaNoAkaneChan"
    />
  </div>
</template>

<script>
import work from './work.vue'

export default {
  name: 'Wagayakane',
  components: {
    work
  }
}
</script>

<style scoped>

</style>
