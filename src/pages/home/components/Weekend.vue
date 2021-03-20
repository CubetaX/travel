<template>
    <div class="container">
        <img class="img" src="http://img1.qunarzz.com/sight/source/1510/6e/1ea71e2f04e.jpg_r_640x214_aa6f091d.jpg" alt="">
        <div class="info-wrapper">
            <p class="info-titile">这ssssssssssssssss是一个段落</p>
            <p class="info-desc">这是一个段落</p>
        </div>
    </div>

</template>

<script>
    export default {
        name: "Weekend"
    }
</script>

<style lang="stylus" scoped>
    .container
        .img
            width 100%
            height 2.5rem
        .info-wrapper
            height .5rem
            text-align left
            padding .2rem
            line-height .4rem
            .info-desc
                color #ccc
                overflow hidden
                white-space nowrap
                text-overflow ellipsis
</style>