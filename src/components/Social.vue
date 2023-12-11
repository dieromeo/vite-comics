<script>
export default {
    name: 'Social',
    data() {
        return {
            title: 'follow up',
            socials: [
                { name: 'Facebook', src: '../../img/footer-facebook.png', link: '#' },
                { name: 'Twitter', src: '../../img/footer-twitter.png', link: '#' },
                { name: 'Youtube', src: '../../img/footer-youtube.png', link: '#' },
                { name: 'Pinterest', src: '../../img/footer-pinterest.png', link: '#' },
                { name: 'Maps', src: '../../img/footer-periscope.png', link: '#' },
            ]
        }
    }
}
</script>

<template>
    <div>
        <h2>{{ title.toUpperCase() }}</h2>
        <ul class="menu">
            <li v-for="social in socials">
                <a :href="social.link"><img :src="social.src" :alt="social.name"></a>
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;

div {
    display: flex;
    align-items: center;

    h2 {
        color: $button-br;
        font-size: 18px;
        margin-right: 30px;
    }

    .menu {
        gap: 20px;
    }
}
</style>