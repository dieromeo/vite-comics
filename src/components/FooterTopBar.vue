<script>
import DcComicsMenu from './DcComicsMenu.vue';
import DcMenu from './DcMenu.vue';
import ShopMenu from './ShopMenu.vue';
import SitesMenu from './SitesMenu.vue';

export default {
    name: 'TopBar',
    components: {
        DcComicsMenu,
        DcMenu,
        ShopMenu,
        SitesMenu,
    }
}
</script>

<template>
    <div class="top-bar">
        <div class="container">
            <div class="left">
                <div>
                    <DcComicsMenu></DcComicsMenu>
                    <ShopMenu></ShopMenu>
                </div>
                <div>
                    <DcMenu></DcMenu>
                </div>
                <div>
                    <SitesMenu></SitesMenu>
                </div>
            </div>
            <div class="right">
                <img src="../../public/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>
</template>

<style lang="scss">
@use '../style/main.scss' as *;

.top-bar {
    background-image: url('../../public/img/footer-bg.jpg');
    background-size: cover;

    h2 {
        color: $titles;
        font-size: 18px;
    }

    ul {
        margin: 20px 0;
    }

    li {
        list-style: none;
        margin-bottom: 5px;
    }

    a {
        text-decoration: none;
        color: $footer-list;
        font-size: 12px;
    }

    .container {
        display: flex;
        align-items: center;
        justify-content: space-between;
        position: relative;
        overflow: hidden;
        padding: 45px 0 40px 0;

        .left {
            display: flex;

            div {
                margin-right: 30px;
            }
        }

        .right img {
            position: absolute;
            top: 50%;
            right: 0;
            transform: translateY(-50%);
        }
    }
}
</style>