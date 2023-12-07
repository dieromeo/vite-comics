<script>
export default {
    name: 'Dc',
    data() {
        return {
            title: 'dc',
            contents: [
                { name: 'Terms of Use', link: '#' },
                { name: 'Privacy Policy (New)', link: '#' },
                { name: 'Ad Choising', link: '#' },
                { name: 'Advertising', link: '#' },
                { name: 'Jobs', link: '#' },
                { name: 'Subscriptions', link: '#' },
                { name: 'Talent Workshops', link: '#' },
                { name: 'CPSC Certificates', link: '#' },
                { name: 'Ratings', link: '#' },
                { name: 'Shop Help', link: '#' },
                { name: 'Contact Us', link: '#' },


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