<script>
export default {
    name: 'Sites',
    data() {
        return {
            title: 'sites',
            contents: [
                { name: 'DC', link: '#' },
                { name: 'MAD Magazines', link: '#' },
                { name: 'DC Kids', link: '#' },
                { name: 'DC Universe', link: '#' },
                { name: 'DC Power Visa', link: '#' },
            ]
        }
    }
}
</script>

<template>
    <h2>{{ title.toUpperCase() }}</h2>
    <ul>
        <li v-for="content in contents">
            <a :href="contents.link">{{ content.name }}</a>
        </li>
    </ul>
</template>

<style lang="scss"></style>