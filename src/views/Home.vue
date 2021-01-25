<template lang="pug">
  #home
    //-img alt="Vue logo" src="../assets/logo.png"
    //-HelloWorld msg="Welcome to Your Vue.js App"/
    .nthu NTHU
    .ipta IPTA
    .moreworks more works
    .TechnologyArt Technology Art
    .niFlex
     .g1shu
     .information New Informations
    .saiFlex
     .SomethingAboutIPTA Something About IPTA
     .list.ts 學士班特色_
      .tsText 
        .text 清華是國際頂尖科技大學，加上合校後的藝術學院，具備發展「科技藝術」的卓越條件。
        .text 我們號召臺灣年輕一代的科技藝術學者專家，我們規劃有科技藝術跨域特別課程，並與業界合作推出創意跨域專題。
        div 你，不需猶豫，歡迎你的加入！
     .list.ab 核心能力_
      .abText
        .text 社會關懷與品格實踐能力｜美感認知與經典欣賞能力｜
        .text 自然感知與創新發想能力｜邏輯思辨與語文溝通能力｜
        div 國際觀點與在地行動能力｜資訊掌握與科技應用能力｜
     router-link.list.nl(to="/course") 課程內容_
     .list.sp 春之清華_
    
     
</template>
<style lang="sass">
#home
 width: 1770px
 //max-width: width 100%
 //height: auto
 background-image: url("https://scontent.ftpe5-1.fna.fbcdn.net/v/t1.0-9/131569235_3445317692183431_6034733367559530690_o.jpg?_nc_cat=100&ccb=2&_nc_sid=730e14&_nc_ohc=VxJkE13ak7gAX-dzAqZ&_nc_ht=scontent.ftpe5-1.fna&oh=ff248153c83cb7ca6cf93dc9326e1943&oe=603133DD")
 background-size: cover
 position: relative
 

.nthu
  font-size: 68px
  color: #FFFFFF
  position: absolute
  // margin-left:-1050px
  // margin-top: 500px
  left: 220px
  top: 562px
  font-family: GemunuLibre-Medium
  letter-spacing: 5px

.ipta
  font-size: 96px
  color: #FFFFFF
  //margin-left: -1045px
  //margin-top: -5px
  position: absolute
  width: 217px
  height: 105px
  left:215px
  top: 642px
  font-style: normal
  font-weight: 500
  line-height: 105px
  letter-spacing: 23px
  font-family: GemunuLibre-Medium

.moreworks
  font-size: 22px
  color: #FFFFFF
  //margin-left: -1045px
  //margin-top: -5px
  position: absolute
  width: 172px
  height: 28px
  left: 193px
  top: 972px
  font-family: HammersmithOne
  font-style: normal
  font-weight: normal
  font-size: 22px
  line-height: 27px
  letter-spacing: 0.1em


.TechnologyArt
  font-size: 24px
  color: #FFFFFF
  //margin-left: 0px
  //margin-top: 0px
  position: absolute
  width: 300px
  height: 26px
  left: 181px
  top: 735px
  font-style: normal
  font-weight: 500
  font-size: 24px
  line-height: 26px
  letter-spacing: 0.28em
  font-family: GemunuLibre-Medium

.niFlex
  position: absolute
  width: 506px
  height: 455px
  margin-left: 1264px
  top: 0px
  background: #695667
  
.g1shu
  position: absolute
  width: 315px
  height: 441px
  margin-left: 112px
  top: 2px
  background: url("http://ipta.nthu.edu.tw/wp-content/uploads/2020/10/poster_web.png")
  background-size: cover

.saiFlex
  position: absolute
  width: 506px
  height: 536px
  margin-left: 1264px
  margin-top: 543px
  background: #695667

.information
  position: absolute
  width: 400px
  height: 39px
  margin-left: -180px
  top: 260px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 590
  font-size: 36px
  line-height: 39px
  letter-spacing: 0.2em
  color: #BDB2C0
  transform: rotate(90deg)

.SomethingAboutIPTA
  position: absolute
  width: 500px
  height: 50px
  margin-left: -233px
  top: 300px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 500
  font-size: 36px
  line-height: 39px
  letter-spacing: 0.2em
  color: #BDB2C0
  transform: rotate(90deg)

.ts
  position: absolute
  width: 228.5px
  height: 33.72px
  left: 120px
  top: 115px
  font-size: 36px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 550
  line-height: 39px
  letter-spacing: 0.2em
  color: #EBE1E1
  white-space: nowrap
  z-index: 999
.ts:hover 
  .tsText
    display: block
// .ts:hover + .nl
//   display: none
// .ts:hover +
//   .nl
//     display: none
// .ts:hover +
//   .sp
//     display: none
.tsText
  width: 816px
  background-color: #2c2c2c
  white-space: normal
  line-height: 40px
  font-size: 26px
  text-align: left
  padding: 10px 20px
  float: right
  display: none
  z-index: 99999
.text
  margin-bottom: 50px
.ab
  position: absolute
  width: 228.5px
  height: 33.72px
  left: 100px
  top: 220px
  font-size: 36px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 550
  line-height: 39px
  letter-spacing: 0.2em
  color: #EBE1E1
  white-space: nowrap
  z-index: 998
.ab:hover 
  .abText
    display: block

.abText
  width: 816px
  background-color: #2c2c2c
  white-space: normal
  line-height: 40px
  font-size: 26px
  text-align: left
  padding: 10px 20px
  float: right
  display: none
.text
  margin-bottom: 50px

.nl
  position: absolute
  width: 228.5px
  height: 33.72px
  left: 100px
  top: 330px
  font-size: 36px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 550
  line-height: 39px
  letter-spacing: 0.2em
  color: #EBE1E1
  white-space: nowrap

.sp
  position: absolute
  width: 228.5px
  height: 33.72px
  left: 100px
  top: 440px
  font-size: 36px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 550
  line-height: 39px
  letter-spacing: 0.2em
  color: #EBE1E1
  white-space: nowrap
.list
  cursor: pointer
  text-decoration: none
</style>
<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>
