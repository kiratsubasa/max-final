<template lang="pug">
  #app
    //-#nav
      //-router-link(to="/") Home |
      //-router-link(to="/about") About
    .menuFlex 
     .search
      .searchIcon
     .menuList
       router-link.menu(v-for="item in menuList" :to="{path: '/' + item.id}" :key="item.id")
        .menuItem {{item.title}}
        div(:class="item.isTrue==true? 'secondaryMenu':'noMenu'")
         router-link.secondary(v-for="option in item.secondary" :to="{path: '/' + option.id}" :key="option.id") {{option.title}}
    router-view
</template>
<script>
export default {
  data(){
    return{
      menuList: [
        {title: 'Home', id: ''},
        {title: 'News', id: 'news'},
        {
          title: 'Admission',
          id: '',
          isTrue: true,
          secondary: [
            {title: '|  春之清華獎學金', id: ''},
            {title: '| FB粉絲團', id: ''},
            {title: '| 2020招生',id: ''},
            {title: '| 招生Q&A', id: ''}
          ]
        },
        {
          title: 'Teachers',
          id: 'teachers',
          isTrue: true,
          secondary: [
            {title: '|  學士班', id: 'teachers'},
            {title: '|  藝設系', id: ''},
            {title: '|  音樂系', id: ''},
            {title: '|  電資學院',id: ''}
          ]
        },
        {title: 'Contact', id: 'contact'}
      ]
    }
  }
}
</script>
<style lang="sass">
@font-face 
  font-family: "GemunuLibre-Medium"
  src: local("GemunuLibre-Medium"),url("./fonts/ttf/GemunuLibre-Light.ttf") format("truetype")
#app 
  font-family: Avenir, Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  text-align: center
  color: #2c3e50
  display: flex
  flex-direction: row-reverse
  width: 1920px
  margin: auto
#nav 
  padding: 30px


#nav a 
  font-weight: bold
  color: #2c3e50

#nav a.router-link-exact-active 
  color: #42b983

.menuFlex
  width: 150px
  height:1080px
  background-color: #FFF
  overflow: visible
  z-index: 1000
  float: right
.search
  padding: 35px 50px
  background-color: #5D6874

.searchIcon
  width: 50px
  height:50px
  background-image: url("https://www.flaticon.com/svg/static/icons/svg/622/622669.svg")
  background-size: cover
.menu
  // display: flex
  // flex-direction: row-reverse
  position: relative
  cursor: pointer
  text-decoration: none
  color: #2c3e50
.menu:hover
  .secondaryMenu
    display: block
    display: flex
    flex-direction: column
    justify-content: space-around
.menuItem
  writing-mode: vertical-lr
  text-orientation: mixed
  font-size: 30px

.menuList
  display: flex
  flex-direction: column
  justify-content: space-around
  height: 960px
  align-items: center
  overflow: visible
.secondaryMenu
  width: 320px
  height: 100%
  position: absolute
  right: 34.67px
  top: 0px
  display: none
  font-family: GemunuLibre-Medium
  font-style: normal
  font-weight: normal
  font-size: 24px
  line-height: 30px
  font-weight: 550
  text-align: left
  letter-spacing: 0.1em
  background-color: #5D6874
.secondary
  color: #fff
  text-decoration: none
  
  
</style>
