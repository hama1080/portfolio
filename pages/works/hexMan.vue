<template>
  <div>
    <work
      :screen-shots="['/works/hexMan/playing.png']"
      :technologies="['Unreal Engine 4']"
      title="HexMan"
      date="2016/3"
      description="Unreal Engine 4を利用して作成した2人対戦用ゲーム．上下分割画面で，それぞれのキャラクターを操作．ボンバーマンのように爆弾を設置し，相手を倒すことが目的．操作性は非常に悪い．"
      source-address=""
    />
  </div>
</template>

<script>
import work from './work.vue'

export default {
  name: 'HexMan',
  components: {
    work
  }
}
</script>

<style scoped>

</style>
