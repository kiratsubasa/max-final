<template lang="pug">
    .headerContainer
        .padding.big NT
        .padding.smallContainer
            .small Technology
            .SmallContainer
                .small Art
                .Medium {{pageTitle}}
        .padding.big HU
</template>
<script>
export default {
    props: ['page-title']
}
</script>
<style lang="sass">
.headerContainer
    display: flex
    flex-direction: row
    font-family: GemunuLibre-Medium
    color: #fff
    align-items: center
    margin: 30px
.big
    font-size: 68px
    letter-spacing: .2rem
.smallContainer
    flex-direction: column
    align-items: flex-start
.SmallContainer
    // width: 300px
    display: flex
    flex-direction: row
    flex-wrap: nowrap
    align-items: center
    justify-content: space-between
.small
    font-size: 24px
    letter-spacing: .6rem
.Medium
    font-size: 48px
    color: #000
    letter-spacing: -0.1rem
.padding
    padding-right: 15px
</style>