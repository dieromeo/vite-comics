<script>
export default {
    name: 'MainMenu',
    data() {
        return {
            items: [
                { image: '../../img/buy-comics-digital-comics.png', description: 'Digital comics', link: '#' },
                { image: '../../img/buy-comics-merchandise.png', description: 'Dc Merchandise', link: '#' },
                { image: '../../img/buy-comics-subscriptions.png', description: 'Subscription', link: '#' },
                { image: '../../img/buy-comics-shop-locator.png', description: 'Comic shop locator', link: '#' },
                { image: '../../img/buy-dc-power-visa.svg', description: 'Dc power visa', link: '#' },
            ]
        }
    }
}
</script>

<template>
    <div class="main-menu">
        <div class="container">
            <ul>
                <li v-for="item in items">
                    <div class="prodotto">
                        <img :src="item.image" :alt="item.description">
                        <a :href="item.link">
                            <h4>{{ item.description.toUpperCase() }}</h4>
                        </a>
                    </div>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;

.main-menu {
    background-color: $button-br;
    padding: 50px;
}

.container {
    margin: 0 auto;

    ul {
        display: flex;
        list-style: none;
        gap: 75px
    }

    a {
        text-decoration: none;
        color: $titles;
        font-size: 14px;

        &:hover {
            text-decoration: underline;
        }
    }

    .prodotto {
        display: flex;
        align-items: center;

        img {
            height: 55px;
            max-width: 55px;
            margin-right: 15px;
        }
    }
}
</style>