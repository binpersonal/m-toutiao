<template>
    <div class="layout-container">
<!--        子路由出口-->
        <router-view />

<!--        底部导航-->
        <van-tabbar v-model="active" route >
            <van-tabbar-item icon="home-o" to="/">首页</van-tabbar-item>
            <van-tabbar-item icon="search" to="/qa">问答</van-tabbar-item>
            <van-tabbar-item icon="video-o" to="/video">视频</van-tabbar-item>
            <van-tabbar-item icon="user-o" to="/my">我的</van-tabbar-item>
        </van-tabbar>

    </div>
</template>

<script>
    export default {
        data () {
            return {
                active: 0,
            };
        },
        computed: {},
        create () {},
        mouted () {},
        methods: {}
    }
</script>
<style scoped lang="scss">

</style>