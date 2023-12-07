<script>
export default {
    name: 'DcComics',
    data() {
        return {
            title: 'dc comics',
            contents: [
                { name: 'Characters', link: '#' },
                { name: 'Comics', link: '#' },
                { name: 'Movies', link: '#' },
                { name: 'Tv', link: '#' },
                { name: 'Games', link: '#' },
                { name: 'Videos', link: '#' },
                { name: 'News', link: '#' },
            ]
        }
    }
}
</script>

<template>
    <h2>{{ title.toUpperCase() }}</h2>
    <ul>
        <li v-for="content in contents">
            <a :href="content.link">{{ content.name }}</a>
        </li>
    </ul>
</template>

<style lang="scss"></style>