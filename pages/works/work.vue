<template>
  <el-row>
    <el-col 
      :span="20" 
      :offset="2">

      <el-card class="work-card">
        <el-row>
          <el-col :span="24">
            <h2>{{ title }}</h2>
            <h3>{{ date }}</h3>

            <div class="description">
              <el-row>
                <el-col :md="{span: 16, offset: 4}">
                  <span v-html="description"/>
                </el-col>
              </el-row>
            </div>

            <div class = "screen-shots">
              <div v-if="screenShots.length === 0"/>
              <div v-else-if="screenShots.length === 1">
                <img 
                  :src="screenShots[0]" 
                  style="max-width: 100%">
              </div>
              <div v-else>
                <el-carousel 
                  :height="carouselHeight" 
                  :autoplay="false" 
                  trigger="click" 
                  indicator-position="outside">
                  <el-carousel-item 
                    v-for="(path, index) in screenShots" 
                    :key="index">
                    <img 
                      :src="path" 
                      style="max-width: 100%">
                  </el-carousel-item>
                </el-carousel>
              </div>
            </div>

            <div v-if="technologies.length > 0">
              <div class="sub-header">Technologies</div>
              <span 
                v-for="(technology, index) in technologies" 
                :key="index" 
                class="tech">
                {{ technology }}
              </span>
            </div>

            <div v-if="publications.length > 0" >
              <div class="sub-header">Publications</div>
              <div
                v-for="(publication, index) in publications"
                :key="index"
                class="publication">
                {{ publication }}
              </div>
            </div>

            <sourceLink 
              v-if="sourceAddress!==''" 
              :address="sourceAddress"/>
          </el-col>
        </el-row>

      </el-card>

    </el-col>
  </el-row>
</template>

<script>
import sourceLink from './sourceLink.vue'

export default {
  name: 'Portfolio',
  components: {
    sourceLink
  },
  props: {
    title:{
      type: String,
      default: 'title'
    },
    date:{
      type: String,
      default: '20xx'
    },
    description: {
      type: String,
      default: 'description'
    },
    screenShots: {
      type: Array,
      default: function(){
        return []
      }
    },
    technologies:{
      type: Array,
      default: function(){
        return []
      }
    },
    publications:{
      type: Array,
      default: function(){
        return []
      }
    },
    sourceAddress:{
      type: String,
      default: ''
    }
  },
  data () {
    return {
      carouselHeight: '300px'
    }
  },
  created: function () {
    if (process.browser) {
      this.resizeWindow()
      window.addEventListener('resize', this.resizeWindow, false)
    }
  },
  beforeDestroy: function () {
    if (process.browser) {
      window.removeEventListener('resize', this.resizeWindow, false)
    }
  },
  methods: {
    resizeWindow: function () {
      if (process.browser) {
        if (window.innerWidth < 768) {
          this.carouselHeight = '150px'
        } else {
          this.carouselHeight = '300px'
        }
      }
    }
  },
}
</script>

<style scoped>
.work-card{
  margin: 0 0 50px 0;
}

.description{
  text-align: left;
}
.description, .screen-shots, .description{
  margin: 30px 0;
}

.sub-header{
  margin: 10px 0;
  font-weight: bold;
}
.tech{
  margin: 0 5px;
}
.publication{
  margin: 0 20px;
  text-align: left;
}
</style>
