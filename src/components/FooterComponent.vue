<script>
import FooterBottomBar from './FooterBottomBar.vue';
import FooterTopBar from './FooterTopBar.vue';

export default {
    name: 'Footer',
    components: {
        FooterBottomBar,
        FooterTopBar
    }
}
</script>

<template>
    <footer>
        <FooterTopBar></FooterTopBar>
        <FooterBottomBar></FooterBottomBar>
    </footer>
</template>

<style lang="scss"></style>