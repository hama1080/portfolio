<template>
  <div>
    <work
      :screen-shots="['/works/fileViewer/animation.gif', '/works/fileViewer/figure0.png', '/works/fileViewer/figure1.png']"
      :technologies="['C++', 'MFC']"
      title="File Viewer"
      date="2012"
      description="
      ファイルの階層構造を、エクスプローラーとは違った形式で表示したメディアアート作品。
      あるディレクトリに含まれるディレクトリは中央付近で回転し、ファイルは周囲を飛び回る。
      操作感は非常に悪いが、見た目的には楽しいものとなっている。
      "
      source-address=""
    />
  </div>
</template>

<script>
import work from './work.vue'

export default {
  name: 'FileViewer',
  components: {
    work
  }
}
</script>

<style scoped>

</style>
