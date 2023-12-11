<script>
export default {
    name: 'Header-menu',
    data() {
        return {
            menu: [
                { name: 'Characters', link: '#', status: false },
                { name: 'Comics', link: '#', status: true },
                { name: 'Movies', link: '#', status: false },
                { name: 'Tv', link: '#', status: false },
                { name: 'Games', link: '#', status: false },
                { name: 'Collectibles', link: '#', status: false },
                { name: 'Videos', link: '#', status: false },
                { name: 'Fans', link: '#', status: false },
                { name: 'News', link: '#', status: false },
                { name: 'Shop', link: '#', status: false },
            ]
        }
    }
}
</script>

<template>
    <ul class="menu">
        <li v-for="element in menu" :class="element.status === true ? 'active' : ''"><a :href="element.link">{{
            element.name.toUpperCase() }}</a></li>
    </ul>
</template>

<style lang="scss">
@use '../style/main.scss' as *;

.menu {
    display: flex;
    list-style: none;
    gap: 35px;
    align-items: center;

    li {
        line-height: 7.5;
    }

    a {
        text-decoration: none;
        color: black;
        font-size: 11px;

        &:hover {
            text-decoration: underline;
        }
    }
}
</style>