<script>
import MainContent from './MainContent.vue';
import MainMenu from './MainMenu.vue';
export default {
    name: 'Main',
    components: {
        MainContent,
        MainMenu
    }
}
</script>
<template>
    <main>
        <MainContent></MainContent>
        <MainMenu></MainMenu>
    </main>
</template>
<style lang="scss"></style>