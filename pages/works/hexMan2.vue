<template>
  <div>
    <work
      :screen-shots="['/works/hexMan2/title.png', '/works/hexMan2/charactor_select.png', '/works/hexMan2/playing.png']"
      :technologies="['Unreal Engine 4']"
      title="HexMan2"
      date="2017/3"
      description="
      HexMan待望の第二作。
      Unreal Engine 4を利用して作成した2人対戦用ゲーム。
      アイスクライマーのように上へと登っていきつつ、ボンバーマンのように爆弾を置き、相手を倒すことが目的。
      所々に崩れる床や、便利アイテムを配置することで、ゲームに面白みを付加している。
      "
      source-address=""
    />
  </div>
</template>

<script>
import work from './work.vue'

export default {
  name: 'HexMan2',
  components: {
    work
  }
}
</script>

<style scoped>

</style>
