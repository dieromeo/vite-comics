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
        <div class="container">
            <Logo></Logo>
            <HeaderMenu></HeaderMenu>
        </div>
    </header>
</template>

<style lang="scss">
.container {
    width: 1260px;
    margin: 0 auto;
}

header .container {
    display: flex;
    align-items: center;
    justify-content: space-between;
}
</style>