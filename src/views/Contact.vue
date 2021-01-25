<template lang="pug">
    .pageContainer
        Header(:page-title='pageTitle')
        .innerContainer
            .add ADD:
              .addmail 30014
              .addd 新竹市南大路521號
            .tel Tel:
            .tell 886-3-5715131#78802 
            .mail Mail:
            .maill ipta@my.nthu.edu.tw
            .say SAY HELLO ON:
            .sayy Instagram
            el-link(href=" https://www.instagram.com/ipta.lab/" target="_blank")
            head
             link(href="https://fonts.googleapis.com/css?family=Oswald:300", rel:'stylesheet', type:'text/css')
            body
             form.form 
              .field.name.active
               label Name 
               input
              .field.email
               label  phone
               input
              .field.password
               label Problem
               input
    //-  .MD 30014
    //-  .addd 新竹市南大路521號
</template>
<script>
import Header from '../components/Header.vue'
export default {
    components: {
        Header
    },
    data(){
        return {
            pageTitle: 'Contact'
        }
    }
}

</script>

<style lang="sass">
.add 
  width: 69px
  height: 47px
  left: 140px
  top: 207px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 500
  font-size: 43px
  line-height: 47px
  color: #000000
  position: absolute
.addmail
  width: 333px
  height: 91px
  left: -115px
  top: 50px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 500
  font-size: 43px
  line-height: 47px
  color: #B5ACB4
  position: absolute
.addd
  position: absolute
  width: 400px
  height: 91px
  left: -26px
  top: 100px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 500
  font-size: 43px
  line-height: 47px
  color: #B5ACB4
.tel
  position: absolute
  width: 52px
  height: 47px
  left: 143px
  top: 398px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 500
  font-size: 43px
  line-height: 47px
  color: #000000
.tell
  position: absolute
  width: 412px
  height: 47px
  left: 117px
  top: 456px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 500
  font-size: 43px
  line-height: 47px
  color: #B5ACB4

.mail
  position: absolute
  width: 72px
  height: 47px
  left: 140px
  top: 562px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 500
  font-size: 43px
  line-height: 47px
  color: #000000

.maill
  position: absolute
  width: 319px
  height: 47px
  left: 140px
  top: 608px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 500
  font-size: 43px
  line-height: 47px
  color: #B5ACB4
.say
  position: absolute
  width: 364px
  height: 94px
  left: 70px
  top: 724px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 500
  font-size: 40px
  line-height: 44px
  color: #000000
.sayy
  position: absolute
  width: 364px
  height: 94px
  left: 35px
  top: 774px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 500
  font-size: 43px
  line-height: 47px
  color: #B5ACB4

.el-link
  position: absolute
  width: 170px
  height: 64px
  left: -630px
  top: 754px
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: 500
  font-size: 40px
  line-height: 97px
  color: #0000

body 
  background-color: #6D4C6A
  font-family: 'Oswald'
  margin: 0
  
  

body:before 
    content: " "
    position: absolute
    background: url(http://distilleryimage1.ak.instagram.com/45bddbe4d57d11e2bf2722000a1fbc66_7.jpg)
    background-size: cover
    z-index: -1
    height: 100
    width: 100%
    -webkit-filter: blur(40px)


form 
  margin-top: 60px


.field 
  // -webkit-filter: blur(2px)
  width: 350px
  padding: 30px
  margin: 0px auto
  background: rgba(#000,0.4)
  // -webkit-transform: scale(0.8)
  // -webkit-transition: -webkit-transform 500ms ease-in-out
  

  &.active 
    -webkit-transform: scale(1)
    -webkit-filter: blur(0)
  


input 
  padding: 12px
  width: 170px
  background: rgba(#fff, 0.4)
  border: 1px solid rgba(#000, 0.8)
    
  &:focus 
    background: rgba(#fff, 0.8)
    outline: none
  


label 
  color: rgba(#fff, 0.4)
  text-align: right
  padding: 0 10px 0 0
  display: inline-block
  text-transform: uppercase
  width: 80px
  font-size: 16px
  letter-spacing: 1px
.form
  position: absolute
  top: 153px
  left: 930px
</style>