<script>
import Logo from './Logo.vue';
import HeaderMenu from './HeaderMenu.vue';
export default {
    name: 'Header',
    components: {
        Logo,
        HeaderMenu
    }
}
</script>
<template>
    <header>
        <Logo></Logo>
        <HeaderMenu></HeaderMenu>
    </header>
</template>
<style lang="scss">
header {
    display: flex;
    align-items: center;
    justify-content: space-around;
}
</style>