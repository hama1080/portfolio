<template>
  <div>
    <work
      :screen-shots="['/works/reversi/figure0.png', '/works/reversi/figure1.png', '/works/reversi/figure2.png']"
      :technologies="['C', 'GrWin']"
      title="リバーシ"
      date="2011"
      description="C言語+GrWinで作成したリバーシ(オセロ)ゲーム．αβアルゴリズムを利用した簡単なCPUも搭載している．"
      source-address=""
    />
  </div>
</template>

<script>
import work from './work.vue'

export default {
  name: 'Reversi',
  components: {
    work
  }
}
</script>

<style scoped>

</style>
