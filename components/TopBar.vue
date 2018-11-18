<template>
  <div id="menu">
    <el-menu 
      :default-active="activeIndex" 
      :router="true" 
      mode="horizontal" 
      class="top-bar"
      background-color="#f5f2ed" 
      text-color="#333" 
      active-text-color="#ff6347">
      <el-menu-item 
        class = "item" 
        index="/">About</el-menu-item>
      <el-menu-item 
        class = "item" 
        index="/works">Works</el-menu-item>
      <el-menu-item 
        class = "item" 
        index="/photos">Photos</el-menu-item>
    </el-menu>
  </div>
</template>

<script>
export default {
  name: 'TopBar',
  data () {
    return {
      activeIndex: '/'
    }
  },
  watch: {
    '$route' (to, from) { 
      this.updateActiveIndex()
    }
  },
  created: function () {
    this.updateActiveIndex()
  },
  methods: {
    updateActiveIndex(){
      let path = this.$route.path
      if(path.indexOf('works') != -1){
        this.activeIndex = '/works'
      }else if(path.indexOf('photos') != -1){
        this.activeIndex = '/photos'
      }else{
        this.activeIndex = '/'
      }
    }
  }
}
</script>

<style scoped>
div#menu {
  width:270px;
  margin: 0 auto 30px auto;
}
.el-menu-item.item{
  width: 90px;
  height: 30px;
  line-height: 30px;
  font-size: 100%;
  text-align: center;
}
</style>
