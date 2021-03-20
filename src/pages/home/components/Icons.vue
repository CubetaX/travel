<template>
    <div class="wrapper" >
        <swiper :options="swiperOption" >
        <swiper-slide class="icons" v-for="(page,index) of pages" :key="index" >
            <div class="icon" v-for="item of page" :key="item.id">
                <img :src="item.imgUrl" alt="">
                <p>{{item.desc}}</p>
            </div>
        </swiper-slide>

        </swiper>
    </div>


</template>

<script>
    //
    export default {
        name: "Icons",
        data(){
            return{
                swiperOption:{
                    //pagination: '.swiper-pagination',
                },
                iconList:[{
                    id:1,
                    imgUrl:"https://pages.ctrip.com/hotel_h5/res/img/index-sale.png?20190619144559j",
                    desc:"按钮1"
                },{
                    id:1,
                    imgUrl:"https://pages.ctrip.com/hotel_h5/res/img/index-sale.png?20190619144559j",
                    desc:"按钮2"
                },{
                    id:1,
                    imgUrl:"https://pages.ctrip.com/hotel_h5/res/img/index-sale.png?20190619144559j",
                    desc:"按钮3"
                },{
                    id:1,
                    imgUrl:"https://pages.ctrip.com/hotel_h5/res/img/index-sale.png?20190619144559j",
                    desc:"按钮4"
                },{
                    id:1,
                    imgUrl:"https://pages.ctrip.com/hotel_h5/res/img/index-sale.png?20190619144559j",
                    desc:"按钮5"
                },{
                    id:1,
                    imgUrl:"https://pages.ctrip.com/hotel_h5/res/img/index-sale.png?20190619144559j",
                    desc:"按钮6"
                },{
                    id:1,
                    imgUrl:"https://pages.ctrip.com/hotel_h5/res/img/index-sale.png?20190619144559j",
                    desc:"按钮7"
                },{
                    id:1,
                    imgUrl:"https://pages.ctrip.com/hotel_h5/res/img/index-sale.png?20190619144559j",
                    desc:"按钮8"
                },{
                    id:1,
                    imgUrl:"https://pages.ctrip.com/hotel_h5/res/img/index-sale.png?20190619144559j",
                    desc:"按钮9"
                }]
            }
        },
        computed:{
            pages(){
                const pages = [];
                this.iconList.forEach((item,index)=>{
                    const page = Math.floor(index/8)
                    if (!pages[page]){
                        pages[page]=[]
                    }
                    pages[page].push(item)
                });
                return pages;
            }
        }
    }
</script>

<style lang="stylus" scoped>
    .icons
        display flex
        flex-wrap wrap
       .icon
            width 25vw
</style>