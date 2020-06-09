<template>
    <div class="header">
        <!-- 顶部导航栏 -->
        <div class="nav-topbar">
            <div class="container">
                <!-- 顶部导航右边内容 -->
                <div class="topbar-menu">
                    <a href="#">小米商城</a>
                    <a href="#">MIUI</a>
                    <a href="#">IoT</a>
                    <a href="#">云服务</a>
                    <a href="#">金融</a>
                    <a href="#">有品</a>
                    <a href="#">小爱开放平台</a>
                    <a href="#">企业团购</a>
                    <a href="#">资质证照</a>
                    <a href="#">协议规则</a>
                    <a href="#">下载app</a>
                    <a href="#">Select Location</a>
                </div>
                <!-- 顶部导航左边内容 -->
                <div class="topbar-user">
                    <a href="#">登入</a>
                    <a href="#">注册</a>
                    <a href="#">消息通知</a>
                    <a href="#" class="my-cart"><span class="icon-cart"></span>购物车</a>
                </div>
            </div>
        </div>
        <!-- 顶部导航栏下导航栏 -->
        <div class="nav-header">
            <div class="container">
                <!-- logo -->
                <div class="header-logo">
                    <a href="/#/index"></a>
                </div>
                <!-- nav -->
                <div class="header-nav">
                    <div class="item-menu">
                        <span>小米手机</span>
                        <div class="children"></div>
                    </div>
                    <div class="item-menu">
                        <span>RedMi红米</span>
                        <div class="children"></div>
                    </div>
                    <div class="item-menu">
                        <span>电视</span>
                        <div class="children"></div>
                    </div>
                </div>
                <!-- search -->
                <div class="header-search">
                    search
                </div>
            </div>
        </div>
    </div>
</template>

<script>
  export default{
    name:'nav-header'
  }
</script>

<style lang="scss" scoped>
    @import './../assets/scss/base.scss';

    .header {
        .nav-topbar {
            height: 39px;
            line-height: 39px;
            background-color: #333;
            color: #B0B0B0;
            .container {
                display: flex;
                justify-content:space-between;
                align-items: center;
                a{
                    height: 39px;
                    display: inline-block;
                    color: #B0B0B0;
                    margin-right: 17px;
                }
                .my-cart {
                    width: 110px;
                    height: 39px;
                    background-color: #FF6600;
                    color: #fff;
                    text-align:center;
                    .icon-cart {
                        display: inline-block;
                        width: 16px;
                        height: 12px;
                        background: url('/imgs/icon-cart-checked.png') no-repeat center;
                        background-size: contain;
                        margin-right: 4px;
                    }
                }
            } 
        }
        .nav-header {
            .container {
                height: 112px;
                display: flex;
                justify-content: space-between;
                align-items: center;
                .header-logo {
                    display: inline-block;
                    width: 55px;
                    height: 55px;
                    background-color: #FF6600;
                    a {
                        display: inline-block;
                        width: 110px;
                        height: 55px;
                        &::before {
                            content: '';
                            display: inline-block;
                            width: 55px;
                            height: 55px;
                            background: url('/imgs/mi-logo.png') no-repeat center;
                            background-size: 55px;
                            transition: margin .2s;
                        }
                        &::after {
                            content: '';
                            display: inline-block;
                            width: 55px;
                            height: 55px;
                            background: url('/imgs/mi-home.png') no-repeat center;
                            background-size: 55px;
                        }
                        &:hover::before {
                            margin-left: -55px;
                            transition: margin .2s;
                        }
                    }
                }
                .header-nav {
                    display: inline-block;
                    width: 200px;
                    padding-left: 209px;
                    .item-menu {
                        display: inline-block;
                        color: #333;
                        font-weight: bold;
                        font-size: 16px;
                        line-height: 112px;
                        span {
                            cursor: pointer;
                        }
                        &:hover {
                            
                        }
                    }

                }
            }
        }
    }
</style>