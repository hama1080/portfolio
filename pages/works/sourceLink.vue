<template>
  <el-row>
    <el-col 
      :offset="18" 
      :span="6" 
      :xs="{span: 10, offset: 14}">
      <a :href="address">
        <el-button 
          plain 
          class="link-button">
          <github-icon 
            name="github" 
            class="custom-icon"/>
          <div class="source-text">Source</div>
        </el-button>
      </a>
    </el-col>
  </el-row>
</template>

<script>
import {GithubIcon } from 'vue-feather-icons'

export default{
  name: 'Sourcelink',
  components: {
    GithubIcon 
  },
  props: {
    address: {
      type: String,
      default: ''
    }
  }
}
</script>

<style scoped>
.link-button{
  font-size: 120%;
  padding: 5px 10px;
  margin: 15px;
}

.v-icon,
.custom-icon {
  width: 20px;
}
</style>
