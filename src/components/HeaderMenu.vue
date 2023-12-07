<script>
export default {
    name: 'Header-menu',
    data() {
        return {
            menu: [
                { name: 'Characters', link: '#' },
                { name: 'Comics', link: '#' },
                { name: 'Movies', link: '#' },
                { name: 'Tv', link: '#' },
                { name: 'Games', link: '#' },
                { name: 'Collectibles', link: '#' },
                { name: 'Videos', link: '#' },
                { name: 'Fans', link: '#' },
                { name: 'News', link: '#' },
                { name: 'Shop', link: '#' },
            ]
        }
    }
}
</script>

<template>
    <ul class="menu">
        <li v-for="element in menu"><a :href="element.link">{{ element.name.toUpperCase() }}</a></li>
    </ul>
</template>

<style lang="scss">
.menu {
    display: flex;
    list-style: none;
    gap: 35px;
    height: 100%;

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