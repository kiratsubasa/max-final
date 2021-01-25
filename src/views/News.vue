<template lang="pug">
    .pageContainer
        Header(:page-title='pageTitle')
        .innerContainer
            .rowNewsContainer
                .newsFlex(v-for="item in news")
                    .newsImg(:style="{'background-image': 'url(' + item.img + ')'}")
                    .newsText
                        .authorAndDate
                            div BY IPTA
                            .newsDate {{item.date}}
                        .tagAndTitle
                            div # {{item.tag}}
                            div {{item.title}}
                        .readMore Read More
            .newsLine 
            .columnNewsFlex
                .news2Flex(v-for="item in news2")
                    .news2Img(:style="{'background-image': 'url(' + item.img + ')'}")
                    .news2Text
                        .tagAndTitle # {{item.title}}
                        .moreAndDate
                            .readMore2 Read more
                            .whiteLine |
                            .blackLine |
                            .newsDate {{item.date}}
</template>
<script>
import Header from '../components/Header.vue'
export default {
    components: {
        Header
    },
    data(){
        return {
            pageTitle: 'News',
            news: [
                {img: 'https://ipta.nthu.edu.tw/wp-content/uploads/2020/10/banner-360x240.png', date: '1 Day ago', tag: '獲獎', title: '系展得獎名單'},
                {img: 'https://ipta.nthu.edu.tw/wp-content/uploads/2020/05/200528-360x240.jpg', date: '8 Months ago', tag: '演講', title: '從腦科學看藝術'},
                {img: 'http://ipta.nthu.edu.tw/wp-content/uploads/2017/10/2018_ipta-poster-1.jpg', date: '3 Years ago', tag: '學士班', title: '跨域招生海報'}
            ],
            news2: [
                {img: 'https://ipta.nthu.edu.tw/wp-content/uploads/2020/02/fb_banner_cut-360x240.png', date: '10 months ago', tag: '獲獎', title: '2020 個人申請第二階段甄選'},
                {img: 'https://ipta.nthu.edu.tw/wp-content/uploads/2019/01/2019-SyntheticMediart-360x240.jpg', date: '9 months ago', tag: '演講', title: '科技藝術策展人講座'},
                {img: 'https://ipta.nthu.edu.tw/wp-content/uploads/2020/03/Yea-chen4-360x240.jpg', date: '11 months ago', tag: '學士班', title: '國際專題演講與工作坊'},
                {img: 'https://ipta.nthu.edu.tw/wp-content/uploads/2020/02/Render-Ghost2-768x510.png', date: '1 year ago', title: '科技物件與人類幻象講座'},
                {img: 'https://ipta.nthu.edu.tw/wp-content/uploads/2019/11/WEB-RGB_p-360x240.jpg', date: '1 year ago', title: '意識與互動藝術論壇'},
                {img: 'https://ipta.nthu.edu.tw/wp-content/uploads/2019/11/001-360x240.jpg', date: '1 year ago', title: '跨國實驗室工作坊'}
            ]
        }
    }
}
</script>
<style lang="sass">
.rowNewsContainer
    display: flex
    flex-direction: row
    margin-top: 50px
    margin-left: 40px
    margin-bottom: 50px
.newsFlex
    display: flex
    flex-direction: row
    margin-right: 100px
.newsImg
    width: 192px
    height: 240px
    background-size: cover
    margin-right: 15px
.newsText
    display: flex
    flex-direction: column
    justify-content: space-between
    text-align: left
    color: #fff
    font-size: 24px
    font-family: GemunuLibre-Medium
.newsDate
    font-size: 18px
.authorAndDate,.readMore
    color: #C7C0C6
.newsLine
    height: 3px
    width: 100%
    background-color: #333
.columnNewsFlex
    display: flex
    flex-direction: row
    flex-wrap: wrap
    margin-top: 50px
    margin-left: 40px
    margin-bottom: 50px
.news2Flex
    display: flex
    flex-direction: column
.news2Img
    width: 270px
    height: 180px
    background-size: cover
    margin-bottom: 15px
    margin-right: 250px
.news2Text
    display: flex
    flex-direction: column
    justify-content: space-between
    text-align: left
    color: #fff
    font-size: 24px
    font-family: GemunuLibre-Medium
.moreAndDate
    display: flex
    flex-direction: row
    align-items: center
    margin-top: 5px
    margin-left: 18px
.newsDate
    color: #333
    margin-left: 30px
.readMore2
    font-size: 18px
    margin-right: 30px
.blackLine
    color: #333
</style>