<template>
  <div>
    <work
      :screen-shots="['/works/vgl/figure0.png','/works/vgl/figure1.png','/works/vgl/figure2.png','/works/vgl/figure3.png']"
      :technologies="['C++', 'PhysX', 'OpenGL(GLSL)', 'WebSocket', 'Qt']"
      :publications="[
        'Performance comparison of physics engines to accelerate house-collapsing simulations, Proc. of IEEE International Symposium on Safety, Security and Rescue Robotics, 2016',
        '物理エンジンの性能評価に基づいたリアルタイム家屋倒壊シミュレーション, 日本機械学会論文集, 2018']"
      title="Virtual Gareki Lab"
      date="2015-2018"
      description="仮想空間上で地震による家屋の倒壊をシミュレーションし，がれきモデルを生成するためのツール．シミュレーションには剛体物理エンジンとしてNVIDIA社のPhysX 3.4を利用し，数千～数万個の剛体から構成されるシミュレーション空間を高速に処理している．また物理演算の過程はOpenGLを用いて描画している．生成したがれきモデルは，がれきモデルの解析や，レスキューロボットシミュレーションなどに利用できる．"
      source-address=""
    />
  </div>
</template>

<script>
import work from './work.vue'

export default {
  name: 'VirtualGarekiLab',
  components: {
    work
  }
}
</script>

<style scoped>

</style>