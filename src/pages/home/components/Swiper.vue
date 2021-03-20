<template>
    <div class="wrapper">
        <swiper :options="swiperOption"  >
            <!-- slides -->
            <!--<swiper-slide ></swiper-slide>
            <swiper-slide ><img class="swiper-img" src="https://dimg04.c-ctrip.com/images/0zg4a120008h700mwF5D1.jpg"/></swiper-slide>
            -->
            <swiper-slide v-for="item of swiperList" :key="item.id">
                <img class="swiper-img" :src="item.imgUrl"/>
            </swiper-slide>
            <swiper-slide>I'm Slide 3</swiper-slide>
            <!-- Optional controls -->
            <div class="swiper-pagination"  slot="pagination"></div>
        </swiper>
    </div>

</template>

<script>
    export default {
        name: "HomeSwiper",

        data (){
            return{
                swiperOption:{
                    pagination: '.swiper-pagination',
                    loop:true
                },
                swiperList:[{
                    id:1,
                    imgUrl:'https://dimg04.c-ctrip.com/images/0zg4a120008h700mwF5D1.jpg'
                },{
                    id:2,
                    imgUrl:'https://dimg04.c-ctrip.com/images/0zg4a120008h700mwF5D1.jpg'
                }]


            }
        }
    }
</script>

<style lang="stylus" scoped>
    .wrapper>>>.swiper-pagination-bullet-active
        background  #cacaca
    .wrapper
        height 0rem
        width 100%
        overflow hidden
        padding-bottom 31.25%
        .swiper-img
            width 100%

</style>