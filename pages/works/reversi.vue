<template>
  <div>
    <work
      title="リバーシ"
      date="2011"
      description="C言語+GrWinで作成したリバーシ(オセロ)ゲーム．αβアルゴリズムを利用した簡単なCPUも搭載している．"
      v-bind:screenShots="['/works/reversi/figure0.png', '/works/reversi/figure1.png', '/works/reversi/figure2.png']"
      v-bind:technologies="['C', 'GrWin']"
      sourceAddress=""
    ></work>
  </div>
</template>

<script>
import work from './work.vue'

export default {
  name: 'reversi',
  components: {
    work
  }
}
</script>

<style scoped>

</style>
