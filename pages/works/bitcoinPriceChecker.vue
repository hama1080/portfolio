<template>
  <div>
    <work
      :screen-shots="['/works/bitcoinPriceChecker/appearance.png']"
      :technologies="['Python', 'Raspberry Pi Zero W', 'Dynamic Lighting System']"
      title="Bitcoin Price Checker"
      date="2017/10"
      description="
      Raspberry Pi Zero Wと、7セグLEDを利用し、現在のビットコイン価格を表示する装置。
      bitflyerのオープンAPIを利用し、取得したビットコイン価格をほぼリアルタイムで表示する。
      小型であるため部屋のインテリアとしても利用可能。"
      source-address="https://github.com/hama1080/PiBitcoinPriceChecker"
    />
  </div>
</template>

<script>
import work from './work.vue'

export default {
  name: 'BitcoinPriceChecker',
  components: {
    work
  }
}
</script>

<style scoped>
</style>
