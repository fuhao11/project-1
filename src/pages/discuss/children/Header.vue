<template>
    <div class="discuss-header">
        <router-link to="/">
            <img src="../../../assets/images/back.png" alt="" class="header-icon">
        </router-link>
        <h3 class="discuss-title">全部评价</h3>
    </div>
</template>

<script>
export default {
    name: "DiscussHeader"
}
</script>

<style lang="stylus">
    .discuss-header
        width:100%
        height 2.3rem
        text-align:center
        line-height:2.3rem
        .header-icon
            width:1.5rem
            height:1.5rem
            position: absolute
            top:.3rem
            left:.4rem
        .discuss-title
            font-size:.84rem
</style>