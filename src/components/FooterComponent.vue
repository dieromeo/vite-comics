<script>
import FooterBottomBar from './FooterBottomBar.vue';

export default {
    name: 'Footer',
    components: {
        FooterBottomBar,
    }
}
</script>

<template>
    <footer>
        <FooterBottomBar></FooterBottomBar>
    </footer>
</template>

<style lang="scss">
footer {
    background-image: url(../../public/img/footer-bg.jpg);
    background-size: cover;
}
</style>