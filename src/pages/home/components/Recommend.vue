<template>
    <div>
        <div class="title">推荐热门</div>
        <div class="container">
            <img class='img' src="http://img1.qunarzz.com/sight/p0/201308/23/b283071686e64dfec8d65eac.jpg_140x140_8c5a7c49.jpg" alt="">
            <div class="info-wrapper">
                <p class="info-titile">这ssssssssssssssss是一个段落</p>
                <p class="info-desc">这是一个段落</p>
                <button class="info-button">查看详情</button>
            </div>
        </div>
    </div>

</template>

<script>
    export default {
        name: "Recommend",
        data(){
           return {}
        }
    }
</script>

<style lang="stylus" scoped>
    .title
        text-align left
        line-height .6rem
        background whitesmoke
        margin-left 5px

    .img
        width 1.7rem
        height 1.7rem
        float left
        padding-right 20px
    .info-wrapper
        text-align left
        line-height .4rem
        .info-titile
            overflow hidden
            white-space nowrap
            text-overflow ellipsis
            padding-top  10px
            font-size .36rem
        .info-button
            margin-top .2rem
            background orange
            color white
            padding .1rem
            border-radius .05rem

</style>