<script>
export default {
    name: 'Shop',
    data() {
        return {
            title: 'shop',
            contents: [
                { name: 'Shop DC', link: '#' },
                { name: 'Shop DC  Collectibles', link: '#' },
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