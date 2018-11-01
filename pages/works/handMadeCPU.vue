<template>
  <div>
    <work
      :screen-shots="['/works/handMadeCPU/figure0.jpg', '/works/handMadeCPU/figure1.jpg']"
      :technologies="['Digital Circuit']"
      title="Hand Made CPU(TD4)"
      date="2012"
      description="'CPUの創り方'に記載の4bit CPUを模倣して作成したCPU．13個のICと，16個のディップスイッチをはんだ付けすることで作成している．ディップスイッチを切り替えることで，自由にプログラムを変更でき，3分のラーメンタイマー等を実行できる．"
      source-address=""
    />
  </div>
</template>

<script>
import work from './work.vue'

export default {
  name: 'HandMadeCPU',
  components: {
    work
  }
}
</script>

<style scoped>

</style>
