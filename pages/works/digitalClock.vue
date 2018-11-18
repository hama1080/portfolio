<template>
  <div>
    <work
      :screen-shots="['/works/digitalClock/figure0.png', '/works/digitalClock/figure1.png', '/works/digitalClock/figure2.png']"
      :technologies="['Arduino', 'Dynamic Lighting System']"
      title="7セグデジタル時計"
      date="2013"
      description="
      Arduinoと7セグメントLEDを用いたデジタル時計。
      4桁の7セグLEDをダイナミック点灯方式を利用し、点灯させている。
      制御基板と表示基板を分けて作成し、立体的に連結することで、スタイリッシュなデザインとしている。
      ケースはスモークのアクリル板と蝶番を組み合わせることにより作成。"
      source-address="https://github.com/hama1080/ArduinoDigitalClock"
    />
  </div>
</template>

<script>
import work from './work.vue'

export default {
  name: 'DigitalClock',
  components: {
    work
  }
}
</script>

<style scoped>

</style>
