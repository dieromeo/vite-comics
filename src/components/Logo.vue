<script>
export default {
    name: 'logo',
    data() {
        return {
            logo: {
                immagine: '../../img/dc-logo.png',
                alt: 'logo dc'
            }
        }
    }
}
</script>

<template>
    <div><img :src="logo.immagine" :alt="logo.alt"></div>
</template>

<style lang="scss" scoped>
img {
    margin: 20px 0;
    height: 80px;
}
</style>