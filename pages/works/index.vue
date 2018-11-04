<template>
  <div>
    <div 
      v-for="(work, index) in works" 
      :key="index">
      <nuxt-link :to="work.detail_path">
        <el-card 
          :body-style="{ padding: '0px' }" 
          class="work-card">
          <img :src="work.img_src">
          <div class="card-text">
            <div class="work-title">{{ work.name }}</div>
            <div class="work-date-wrap"><div class="work-date"><calendar-icon 
              name="calendar" 
              class="custom-icon"/>{{ work.date }}</div></div>
          </div>
        </el-card>
      </nuxt-link>
    </div>
  </div>
</template>

<script>
import {CalendarIcon } from 'vue-feather-icons'

export default {
  name: 'Works',
  components: {
    CalendarIcon 
  },
  data () {
    return {
      works: [
        {
          date: '2018/6',
          name: 'ポートフォリオサイト',
          img_src: '/works/portfolio/eyecatch.png',
          detail_path: '/works/portfolio'
        },
        {
          date: '2017-2018',
          name: 'Virtual Gareki Lab',
          img_src: '/works/vgl/eyecatch.png',
          detail_path: '/works/vgl'
        },
        {
          date: '2018/3',
          name: 'ひらがなGAN',
          img_src: '/works/hiraganaGAN/eyecatch.png',
          detail_path: '/works/hiraganaGAN'
        },
        {
          date: '2017/10',
          name: 'Bitcoin Price Checker',
          img_src: '/works/bitcoinPriceChecker/eyecatch.png',
          detail_path: '/works/bitcoinPriceChecker'
        },
        {
          date: '2017/8',
          name: '我が家の茜ちゃんPJ',
          img_src: '/works/wagayakane/eyecatch.png',
          detail_path: '/works/wagayakane'
        },
        {
          date: '2017/3',
          name: 'HexMan2',
          img_src: '/works/hexMan2/eyecatch.png',
          detail_path: '/works/hexMan2'
        },
        {
          date: '2016/11',
          name: 'お天気掲示板',
          img_src: '/works/forecastBoard/eyecatch.png',
          detail_path: '/works/forecastBoard'
        },
        {
          date: '2016/3',
          name: 'HexMan',
          img_src: '/works/hexMan/eyecatch.png',
          detail_path: '/works/hexMan'
        },
        // {
        //   date: '2014/7',
        //   name: 'タイマーレリーズ',
        //   img_src: '/logo.png',
        //   detail_path: '/works/timerRelease'
        // },
        {
          date: '2013',
          name: '7セグデジタル時計',
          img_src: '/works/digitalClock/eyecatch.png',
          detail_path: '/works/digitalClock'
        },
        {
          date: '2012',
          name: 'Hand Made CPU(TD4)',
          img_src: '/works/handMadeCPU/eyecatch.png',
          detail_path: '/works/handMadeCPU'
        },
        {
          date: '2012',
          name: 'File Viewer',
          img_src: '/works/fileViewer/eyecatch.png',
          detail_path: '/works/fileViewer'
        },
        {
          date: '2011',
          name: 'リバーシ',
          img_src: '/works/reversi/eyecatch.png',
          detail_path: '/works/reversi'
        }
      ]
    }
  }

}
</script>

<style scoped>
.work-card{
  width: 250px;
  height: 280px;
  margin: 30px;
  padding-top: 20px;
  float: left;
}

.card-text{
  padding: 20px;
}
.work-title{
  font-size: 120%;
  line-height: 28px;
  font-weight: bold;
}
.v-icon,
.custom-icon {
  width: 14px;
  margin: 0 4px 0 0;
}
.work-date{
  color: #AAA;
  display: flex;
  align-items: center;
}
.work-date-wrap{
  display: flex;
  justify-content: flex-end;
}
</style>
