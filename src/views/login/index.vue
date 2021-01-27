<template>
    <div class="login-container">
        <van-nav-bar
                title="登录"
                left-arrow
                @click-left="onClickLeft"
                @click-right="onClickRight"
        />
        <van-cell-group>
            <van-field
                    v-model="value1"
                    type="number"
                    left-icon="phone-circle-o"
                    placeholder="手机号"
            />
            <van-field
                    v-model="password"
                    type="password"
                    left-icon="closed-eye"
                    placeholder="密码"
            >
                <template #button>
                    <van-button size="small" type="default">发送验证码</van-button>
                </template>
            </van-field>
        </van-cell-group>
        <van-button type="info" block style="width: 90%;margin: 30px auto">登录</van-button>
        <!--       小智同学-->
    </div>
</template>

<script>
    import {Toast} from 'vant';

    export default {
        data() {
            return {}
        },
        computed: {},
        create() {
        },
        mouted() {
        },
        methods: {
            onClickLeft() {
                Toast('返回');
            },
            onClickRight() {
                Toast('按钮');
            },
        }
    }
</script>
<style scoped lang="scss">
    .login-container {
        background: #EDEDED;
        height: 100vh;

    }
</style>