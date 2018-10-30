<template>
  <div>
    <el-row>
      <el-col :span="24">
        <el-card class="photo-card">
          <img src="/photos/poonhill.jpg" class="photo">
          <div class="photo-detail">Poon Hill, Nepal</div>
        </el-card>
      </el-col>
    </el-row>

    <el-row>
      <el-col :span="10" :offset="1" :xs="{span: 24, offset: 0}">
        <el-card class="photo-card">
          <img src="/photos/drop0.jpg" class="photo">
        </el-card>
      </el-col>
      <el-col :span="10" :offset="2" :xs="{span: 24, offset: 0}">
        <el-card class="photo-card">
          <img src="/photos/drop1.jpg" class="photo">
        </el-card>
      </el-col>
    </el-row>

    <el-row>
      <el-col :span="24">
        <el-card class="photo-card">
          <img src="/photos/hokuryu.jpg" class="photo">
          <div class="photo-detail">Hokuryu, Hokkaido, Japan</div>
        </el-card>
      </el-col>
    </el-row>

    <el-row>
      <el-col :span="24">
        <el-card class="photo-card">
          <img src="/photos/biei.jpg" class="photo">
          <div class="photo-detail">Biei, Hokkaido, Japan</div>
        </el-card>
      </el-col>
    </el-row>

    <el-row>
      <el-col :span="24">
        <el-card class="photo-card">
          <img src="/photos/abashiri.jpg" class="photo">
          <div class="photo-detail">Abashiri, Hokkaido, Japan</div>
        </el-card>
      </el-col>
    </el-row>

    <el-row>
      <el-col :span="24">
        <el-card class="photo-card">
          <img src="/photos/varanasi.jpg" class="photo">
          <div class="photo-detail">Varanasi, India</div>
        </el-card>
      </el-col>
    </el-row>

    <el-row id="social">
      <el-col :span="24">
        <a href="https://www.instagram.com/hama1080_/"><instagram-icon name="instagram" class="custom-icon"></instagram-icon></a>
      </el-col>
    </el-row>

  </div>
</template>

<script>
import {InstagramIcon} from 'vue-feather-icons'

export default {
  name: 'Photographs',
  components: {
    InstagramIcon
  }
}
</script>

<style scoped>
.photo-card{
  margin: 20px 5px;
}

.photo{
  width: 100%;
}

.photo-detail{
  color: #AAA;
  font-size: 75%;
  float: right;
}

.v-icon,
.custom-icon {
  width: 30px;
  margin: 20px 0;
}

a:link { color: #333; }
a:visited { color: #333; }
a:hover { color: #ff6347; }
a:active { color: #ff6347; }
</style>
