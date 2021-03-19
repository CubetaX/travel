<template>
    <div class="header">
        <div class="header-left">
            <div class="iconfont">&#xe624;</div>
        </div>
        <div class="header-input">
            <span class="iconfont">&#xe632;</span>输入搜索名称
        </div>
        <div class="header-right">城市
            <span class="iconfont arrow">&#xe64a;
            </span>
        </div>
    </div>

</template>

<script>
    export default {
        name: "header"
    }
</script>

<style lang="stylus" scoped>
    @import "~styles/var.styl"
    .header
        display flex
        line-height  .86rem
        background $bgColor
        color #ffffff
        .header-left
            width .64rem
            float left
        .header-input
            color #333333
            text-align left
            flex 1
            height 0.64rem
            line-height 0.64rem
            margin-top 0.12rem
            margin-bottom 0.12rem
            margin-left 0.2rem
            padding-left 0.2rem
            background white

        .header-right
            float right
            width 1.24rem
            .arrow
                font-size .24rem

</style>