<template>
  <div v-show="show">
    <el-row>
      <el-col :span="24">
        <img src="/profile_picture.png">
        <h1>@hama1080</h1>
        <h1>Takuto Hamano</h1>
        <h2>Software engineer with the knowledge of hardware.</h2>
      </el-col>
    </el-row>

    <el-row id="skills">
      <el-col :span="24">
        <div class="skill-header">Skills</div>
        <span class="skill">C/C++</span>
        <span class="skill">Python</span>
        <span class="skill">PhysX</span>
        <span class="skill">Electronics</span>
      </el-col>
    </el-row>

    <el-row id="social">
      <el-col :span="24">
        <a href="https://github.com/hama1080"><github-icon class="custom-icon"/></a>
        <a href="https://twitter.com/hama1080"><twitter-icon 
          name="twitter" 
          class="custom-icon"/></a>
        <a href="https://www.instagram.com/hama1080_/"><instagram-icon 
          name="instagram" 
          class="custom-icon"/></a>
        <a href="https://www.linkedin.com/in/takutohamano/"><linkedin-icon 
          name="linkedin" 
          class="custom-icon"/></a>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import { GithubIcon , TwitterIcon, InstagramIcon, LinkedinIcon} from 'vue-feather-icons'

export default {
  name: 'Profile',
  components: {
    GithubIcon,
    TwitterIcon,
    InstagramIcon,
    LinkedinIcon
  },
  data () {
    return {
      show: true
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#skills{
  margin: 20px 0;
}
#social{
  margin: 40px 0;
}

.skill-header{
  margin: 10px 0;
  font-size: 120%;
  font-weight: bold;
}
.skill{
  font-size: 120%;
  margin: 0 10px;
}

.v-icon,
.custom-icon {
  width: 30px;
  margin: 0 10px;
}

a:link { color: #333; }
a:visited { color: #333; }
a:hover { color: #ff6347; }
a:active { color: #ff6347; }
</style>
