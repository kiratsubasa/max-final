<template lang="pug">
    .pageContainer
        Header(:page-title='pageTitle')
        .innerContainer
          .d1h #課程設計兼顧跨領域（transdisciplinary）與多領域（multi-disciplinary）
          .d2h 學位：科技藝術學士學位 （Bachelor of Science and Art）
          .d3h 第二專長學士學位（若學生有另選第二專長課程）
          .d4h 藝術學院學士班108學年度入學必修科目、學分數暨畢業總學分表
          img.courseImg(src="https://scontent.ftpe5-1.fna.fbcdn.net/v/t1.0-9/142094572_3527282550653611_5763948029344504671_o.jpg?_nc_cat=104&ccb=2&_nc_sid=730e14&_nc_ohc=bn8ynQgWnw8AX_qkdhk&_nc_ht=scontent.ftpe5-1.fna&oh=83e999f14a5a5f7a4a7b9295fd8e6a26&oe=6033E782")
</template>
<script>
import Header from '../components/Header.vue'
export default {
    components: {
        Header
    },
    data(){
        return {
            pageTitle: 'Course'
             
        }
    }
}
</script>
<style lang="sass">
.pageContainer
    width: 1770px
    background-color: #664863
    height: 1080px
    position: relative
.innerContainer
    width: 97%
    height: 950px
    background-color: #6D4C6A
    position: absolute
    bottom: 0px
    left: 0px
.d1h
  position: absolute
  width: 1500px
  height: 161px
  left: -180px
  top: 75px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 550
  font-size: 30px
  line-height: 40px
  letter-spacing: 0.05em
  color: #000000

.d2h
  position: absolute
  width: 977px
  height: 100px
  left: -50px
  top: 159px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 550
  font-size: 28px
  line-height: 40px
  letter-spacing: 0.05em
  color: #B5ACB4

.d3h
  position: absolute
  width: 977px
  height: 161px
  left: -70px
  top: 220px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 550
  font-size: 28px
  line-height: 40px
  letter-spacing: 0.05em
  color: #B5ACB4

.d4h
  position: absolute
  width: 650px
  height: 40px
  left: 70px
  top: 308px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 550
  font-size: 20px
  line-height: 40px
  letter-spacing: 0.05em
  color: #000000

.courseImg
  position: absolute
  width: 1120px
  height: 546px
  left: 96px
  top: 358px


</style>