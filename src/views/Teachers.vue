<template lang="pug">
    .pageContainer
        Header(:page-title='pageTitle')
        .innerContainer
            .teacherContainer
                .teacherTitle #藝術學院學士班專任師資
                .teacherLine
                .thr
                    el-carousel(style="margin-top:77px")
                        el-carousel-item(v-for="item in teachers" :key="item")
                            //- div {{item}}
                            .twoTeacherFlex
                                .teacherFlex(v-for="teacher in item")
                                    .teacherImg(:style="{'background-image': 'url(' + teacher.img + ')'}")
                                    .teacherText
                                        .firstZone
                                            .teacherName {{teacher.name}}
                                            .teacher {{teacher.title}}
                                        .secondZone
                                            .teacherExpert(v-for="i in teacher.expert") {{i}}
                .teacherTitle #藝術學院學士班兼任師資
                .teacherLine
                .thr
                    el-carousel(style="margin-top:77px")
                        el-carousel-item(v-for="item in teachers2" :key="item")
                            //- div {{item}}
                            .twoTeacherFlex
                                .teacherFlex(v-for="teacher in item")
                                    .teacherImg(:style="{'background-image': 'url(' + teacher.img + ')'}")
                                    .teacherText
                                        .firstZone
                                            .teacherName {{teacher.name}}
                                            .teacher {{teacher.title}}
                                        .secondZone
                                            .teacherExpert(v-for="i in teacher.expert") {{i}}


</template>
<script>
import Header from '../components/Header.vue'
export default {
    components: {
        Header
    },
    data(){
        return {
            pageTitle: 'Teachers',
            teachers: [
                [
                    {img: 'http://ipta.nthu.edu.tw/-iptaimg/faculty-XN.jpg', name: '許素朱（小牛） (Su-Chu Hsu)', title: '博士/教授 兼 院長', expert: ['互動科技藝術','物聯網創意應用','數位文創產業','創客藝術與教育']},
                    {img: 'http://ipta.nthu.edu.tw/-iptaimg/faculty-Chuyin.jpg', name: '陳珠櫻 (Chu-Yin Chen)', title: '博士/教授 間 班主任', expert: ['數位藝術創作','創作心理學','腦科學','人工生命','認知科學','心理現象學']}
                ],
                [
                    {img: 'http://ipta.nthu.edu.tw/-iptaimg/faculty-Chiu.jpg', name: '邱誌勇 (Chih-Yung Chiu)', title: '博士/教授', expert: ['新媒體藝術美學','藝術評論','電影電視美學與科技文化研究']},
                    {img: 'http://ipta.nthu.edu.tw/wp-content/uploads/2017/09/faculty-Youchuangwen-e1599050882929.png', name: '游創文 (Chuang-Wen You)', title: '博士/助理教授', expert: ['人機互動','普及計算','無線感測網路']}
                ],
                [
                    {img: 'http://ipta.nthu.edu.tw/wp-content/uploads/2017/09/hkchu-e1599051131983.jpg', name: '朱宏國 (Hung-Kuo Chu)', title: '博士/副教授 (資訊工程系合聘)', expert: ['人機互動','AR/VR/MR','Smart Manipulation','Visual Perception','Shape Analysis']},
                    {img: 'http://ipta.nthu.edu.tw/-iptaimg/faculty-Huang.jpg', name: '黃致傑 (Scotte C. C. Huang)', title: '博士/助理教授 (通識教育中心合聘)', expert: ['仿生設計','科技藝術','人機互動','動態建築','產品設計']}
                ],
                [
                    {img: 'http://ipta.nthu.edu.tw/-iptaimg/faculty-Bao.jpg', name: '包盛盈 (Sheng-Ying Pao)', title: '博士/助理教授', expert: ['生命科學','醫學工程','數位媒體藝術','前瞻科技創新創業']},
                    {img: 'http://ipta.nthu.edu.tw/wp-content/uploads/2017/09/messageImage_1565860106157-e1599050953492.jpg', name: '曹存慧 (Tsun-Hui Tsao)', title: '博士/助理教授', expert: ['生物藝術','生物資訊','轉錄體學','基因工程','分子生物學']}
                ]
            ],
            teachers2: [
                [
                    {img: 'http://ipta.nthu.edu.tw/-iptaimg/faculty-ChiHong.png', name: '蔡奇宏 (Chi-Hung Tsai)', title: '講師/科技藝術業界顧問教師', expert: ['光動藝術','互動裝置藝術','策展規劃與執行']},
                    {img: 'http://ipta.nthu.edu.tw/wp-content/uploads/2020/09/Jianrueijen-e1599054462431.jpg', name: '簡瑞瑱 (Ruei-Jen Jian)', title: '講師', expert: ['視覺設計','設計策略','數位藝術評論']}
                ],
                [
                    {img: 'http://ipta.nthu.edu.tw/-iptaimg/faculty-SHihTa.jpg', name: '劉士達 (Shih-Ta Liu)', title: '講師/科技藝術業界顧問教師', expert: ['互動科技研發','電子藝術','互動藝術']},
                    {img: 'http://ipta.nthu.edu.tw/wp-content/uploads/2020/09/07-%E8%8E%8A%E5%BF%97%E7%B6%AD%E5%A4%A7%E9%A0%AD%E7%85%A7-e1599053404704.jpg', name: '莊志維 (Chih-Wei Chuang)', title: '講師/新媒體藝術家', expert: ['裝置藝術','現地創作']}
                ],
                [
                    {img: 'http://ipta.nthu.edu.tw/wp-content/uploads/2020/09/Yehtinghao-e1599054118639.jpg', name: '葉廷皓 (Ting-Hao Yeh)', title: '講師/新媒體藝術家', expert: ['實驗聲響','動態影像程式設計','實景投影']},
                    {img: 'http://ipta.nthu.edu.tw/wp-content/uploads/2020/09/Yushihfu-e1599054266255.jpg', name: '盂施甫 (Shih-Fu Yu)', title: '講師/新媒體藝術家', expert: ['動力藝術','技術美學','數位自造']}
                ],
                [
                    {img: 'http://ipta.nthu.edu.tw/wp-content/uploads/2020/09/Wuchunghaw.jpg', name: '吳中浩 (Chung -Haw Wu)', title: '教授/清華大學資工系專案顧問', expert: ['計算機結構','數字媒體']},
                    {img: 'http://ipta.nthu.edu.tw/wp-content/uploads/2020/09/Jeanclaudehoyami.jpg', name: '歐·尚-克洛德 (Jean-Claude Hoyami)', title: '講師', expert: ['Telecommunication & IP Networks','Computer Graphics & Animation','Computer Science','Artificial Life']}
                ]
            ]
        }
    }
}
</script>
<style lang="sass">
.teacherContainer
    margin-top: 32px
    margin-left: 32px
.teacherTitle
    color: #333
    font-size: 28px
    text-align: left
.teacherLine
    margin: auto
    margin-top: 2px
    width: 1400px
    height: 1px
    background-color: #333
.twoTeacherFlex
    display: flex
    flex-direction: row
.teacherFlex
    display: flex
    flex-direction: row
    width: 760px
.teacherImg
    width: 175px
    height: 196px
    background-size: cover
    border: 28px solid #212121
    margin-right: 28px
.teacherText
    display: flex
    flex-direction: column
    font-size: 28px
    justify-content: space-around
    text-align: left
.teacherName
    color: #fff
.teacher
    color: #333
.secondZone
    display: flex
    flex-direction: row
    flex-wrap: wrap
    max-width: 513px
.teacherExpert
    padding: 0px 10px
    margin: 2px 0px
    border-left: 2px solid #000
    color: #000 
</style>