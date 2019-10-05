<template>
    <div class="discuss-zone">
        <ul>
            <li class="item" v-for="item of list" :key="item.userid">
                <div class="top">
                    <div class="top_left">
                        <span><img class="head" :src="item.head" alt="头像"></span>
                        <div class="name">{{item.name}}</div>
                        <div class="star">
                            <img v-for="innerS in item.star" :key="'a'+innerS" src="../../../assets/images/star.png" alt="">
                            <img v-for="innerG in 5-item.star" :key="'b'+innerG"  src="../../../assets/images/star_gray.png" alt="">
                        </div>
                    </div>
                    <span class="time">{{item.time}}</span>
                </div>
                <div class="content" v-if="!item.content[0].text">此用户没有填写评价</div>
                <div class="content" v-else>{{item.content[0].text}}</div>
                <div :class="[item.content[0].photo.length<3 ? 'imgs-other' : 'imgs']">
                    <img v-for="(inner,index) in item.content[0].photo" :key="index" class="item-img" :src="inner" alt="">
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: "DiscussZone",
    props:['list']
}
</script>

<style lang="stylus">
    .discuss-zone
        width:96%
        height:auto
        margin:1rem auto
        margin-top:0
        .item
            height:auto
            background:#fff
            border-radius:.3rem
            padding:.5rem
            margin-bottom:.5rem
            display:flex
            flex-direction:column
            justify-content:space-between
            .top
                with:100%
                height:1.8rem
                display:flex
                justify-content:space-between
                align-items center
                .top_left
                    display:flex
                    align-items:center
                    .head
                        width:1.5rem
                    .name
                        margin:0 .5rem
            .content
                margin: .5rem 0
                line-height:1rem
            .imgs
                display:flex
                flex-direction:row
                justify-content:space-between
                .item-img
                    width:28%
            .imgs-other
                display:flex
                flex-direction:row
                justify-content:space-around
                .item-img
                    width:28%
</style>